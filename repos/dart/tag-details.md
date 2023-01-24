<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.19`](#dart219)
-	[`dart:2.19-sdk`](#dart219-sdk)
-	[`dart:2.19.0`](#dart2190)
-	[`dart:2.19.0-sdk`](#dart2190-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19`

**does not exist** (yet?)

## `dart:2.19-sdk`

**does not exist** (yet?)

## `dart:2.19.0`

**does not exist** (yet?)

## `dart:2.19.0-sdk`

**does not exist** (yet?)

## `dart:beta`

```console
$ docker pull dart@sha256:8908ea48041319fd2ee7a378a71123e72f200c62a88a7bcae5988f3dc886c46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:117932152a83fec6b7604548394f11e76cf3a84163b524caab4b74bc354da1d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301472777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f6e1822862290c2cb2ae99204c0f80cf35da17783287aea6429e6078510bb4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e10c768f4cacdde82ef48dee4cfbf83f590630802d4936ee179689d721a6d4`  
		Last Modified: Thu, 12 Jan 2023 19:21:44 GMT  
		Size: 222.8 MB (222840614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:8c36e8dbb79ee3e2bbfd12523d047834dd93282f3013e35ec6d61e6e2de8a4b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.7 MB (197659266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1750b61c94d73fa926e25c3db75f51705759a733ae110103e89ab2499299088`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef90b288d9c496e7efb997816b428b40f7cf00e23ac1b687b1edf9fc0d9cc457`  
		Last Modified: Thu, 12 Jan 2023 19:00:08 GMT  
		Size: 128.9 MB (128855733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:67bfda77c3987bcd689528069ee2947b9dae140d1396ecc9f98a201def5519df
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206911993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b229e523b1dae58edae47877582c7e513a67012711c5c1afa3938bbc6e864a15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0351c4614e121c1b7cd6809a6a75cad1a40ba9ed98abe895c0378176ce9df5ab`  
		Last Modified: Thu, 12 Jan 2023 19:41:01 GMT  
		Size: 130.3 MB (130310259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:8908ea48041319fd2ee7a378a71123e72f200c62a88a7bcae5988f3dc886c46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:117932152a83fec6b7604548394f11e76cf3a84163b524caab4b74bc354da1d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301472777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f6e1822862290c2cb2ae99204c0f80cf35da17783287aea6429e6078510bb4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e10c768f4cacdde82ef48dee4cfbf83f590630802d4936ee179689d721a6d4`  
		Last Modified: Thu, 12 Jan 2023 19:21:44 GMT  
		Size: 222.8 MB (222840614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:8c36e8dbb79ee3e2bbfd12523d047834dd93282f3013e35ec6d61e6e2de8a4b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.7 MB (197659266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1750b61c94d73fa926e25c3db75f51705759a733ae110103e89ab2499299088`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef90b288d9c496e7efb997816b428b40f7cf00e23ac1b687b1edf9fc0d9cc457`  
		Last Modified: Thu, 12 Jan 2023 19:00:08 GMT  
		Size: 128.9 MB (128855733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:67bfda77c3987bcd689528069ee2947b9dae140d1396ecc9f98a201def5519df
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.9 MB (206911993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b229e523b1dae58edae47877582c7e513a67012711c5c1afa3938bbc6e864a15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=a7154a06224168546f75b7f6294e9630f18da7ab33d28912a1bc5fab076f9da4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d027251be6f47dbedee07420c054510a8cd9019bbecdb92dcdf9d799f1568a43;             SDK_ARCH="arm";;         arm64)             DART_SHA256=edc4bf48b3bc3999caf8c3093dffffb960369699bc5ab912ebfd153cf02cbd35;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-444.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0351c4614e121c1b7cd6809a6a75cad1a40ba9ed98abe895c0378176ce9df5ab`  
		Last Modified: Thu, 12 Jan 2023 19:41:01 GMT  
		Size: 130.3 MB (130310259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:ff4b8ee44567352ead890bc192699791c7574c67333b72598de830118c960a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:23181026ee0331f929a0bb62d080dfdef0ed8285504e9ca7d873b49a798bb7ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271924749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0271766ac7fed78ad48a5a3470359f81b7534a940fb627270d1679f4f512e815`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b90db08b55e614532290fe1c16f5b73a404671e9d96385ae9f1032e50c041`  
		Last Modified: Thu, 12 Jan 2023 19:20:46 GMT  
		Size: 193.3 MB (193292586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c408066e1a77ccc1647a365f000658498ada4a9b1c66d4ca63340113f0b17b33
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180590064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a4b1b8a1906fae025250dd2dcb1a3b245a4c49368cb1d88dff2eb4818f6b73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Thu, 12 Jan 2023 18:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5accab2c9040cf76fc67ecc5c9213dccc724483116fc8a4d58ecc79bd4f37e4`  
		Last Modified: Thu, 12 Jan 2023 18:59:05 GMT  
		Size: 111.8 MB (111786531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8df48f70026f2548920f9e90c2a7c90c50a9de65ed5964d49605d5d8d8f551bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189543347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a1a63f1cacb1dc969130b9e404a7eeb077d26742ca375b557f923cf8d3e2e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Thu, 12 Jan 2023 19:39:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=337de0ad3ee66dca7ffa81fc3cd9ecd53d4593384da9d1dfcf4b68f69559fa2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=daa5139774ba50f100115c79dc193c0bb0a48737c79eb915ee8f25c4ec74ace1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=684092802f280ca7a64b111da647bbd380d2ce5adf8a23bcd70cc902a3c4a495;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ca91e31f2a43fd7ac898c19795a9b013b61eb6b1b1baf3f4f1ec41c447f29`  
		Last Modified: Thu, 12 Jan 2023 19:40:20 GMT  
		Size: 112.9 MB (112941613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
