<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:3`](#dart3)
-	[`dart:3-sdk`](#dart3-sdk)
-	[`dart:3.0`](#dart30)
-	[`dart:3.0-sdk`](#dart30-sdk)
-	[`dart:3.0.3`](#dart303)
-	[`dart:3.0.3-sdk`](#dart303-sdk)
-	[`dart:3.1.0-63.1.beta`](#dart310-631beta)
-	[`dart:3.1.0-63.1.beta-sdk`](#dart310-631beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:3`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3-sdk`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0-sdk`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0-sdk` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.3`

```console
$ docker pull dart@sha256:f3a08d3647fb35dc736eed396367d3c6a80a469cfb289e68ae3d637de6903900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.3` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.3-sdk`

```console
$ docker pull dart@sha256:f3a08d3647fb35dc736eed396367d3c6a80a469cfb289e68ae3d637de6903900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-63.1.beta`

```console
$ docker pull dart@sha256:ad39648056b76d69619c53dd18d4aa4164e4a26b4fb1104466cf4d614c41e1fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1.0-63.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:3e96bb61088639d6d8ceb2158cfae8d979ffe0502092c071b178175b4ddbb227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297269091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0aa9b4b68f8c9e6026e33f6b799e6da20f466f107d7973eb11b0a4e182043e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Tue, 23 May 2023 02:03:13 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017ed06ffd303ab8d53d1db147213878637053f777eb8653753bcc2631c51f7f`  
		Last Modified: Tue, 23 May 2023 02:04:46 GMT  
		Size: 218.6 MB (218601860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-63.1.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:4641ae6894c36dea2d891ade272dfc7c4a1d7a107a736b9654bbe2e3625b21cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191524171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf54d6f5866203f7a0fc26973af75c47b2a2d158dfd8e6bdb07aa3d3c296e635`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Tue, 23 May 2023 06:33:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b574256fc8a4e147a3ccdfb5e39fee9190b89cf93cb9496783fadeae141135`  
		Last Modified: Tue, 23 May 2023 06:34:30 GMT  
		Size: 122.7 MB (122683473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-63.1.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4a2d4689caaf73bd66fc8f815e9608d98d52c77c0f633e8a7451b951e4ad7fdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.7 MB (200705129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436ad7cf4ae165cce24cc1dc9f6b7f1f2c31e4d1323b7c487a9448faaf57cb77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Tue, 23 May 2023 01:44:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3fff2216e0d2bfb5c1cf9eaa5494ed646c21921dae1b88da22c00dff67af15`  
		Last Modified: Tue, 23 May 2023 01:45:07 GMT  
		Size: 124.1 MB (124080383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-63.1.beta-sdk`

```console
$ docker pull dart@sha256:ad39648056b76d69619c53dd18d4aa4164e4a26b4fb1104466cf4d614c41e1fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1.0-63.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:3e96bb61088639d6d8ceb2158cfae8d979ffe0502092c071b178175b4ddbb227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297269091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0aa9b4b68f8c9e6026e33f6b799e6da20f466f107d7973eb11b0a4e182043e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Tue, 23 May 2023 02:03:13 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017ed06ffd303ab8d53d1db147213878637053f777eb8653753bcc2631c51f7f`  
		Last Modified: Tue, 23 May 2023 02:04:46 GMT  
		Size: 218.6 MB (218601860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-63.1.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4641ae6894c36dea2d891ade272dfc7c4a1d7a107a736b9654bbe2e3625b21cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191524171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf54d6f5866203f7a0fc26973af75c47b2a2d158dfd8e6bdb07aa3d3c296e635`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Tue, 23 May 2023 06:33:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b574256fc8a4e147a3ccdfb5e39fee9190b89cf93cb9496783fadeae141135`  
		Last Modified: Tue, 23 May 2023 06:34:30 GMT  
		Size: 122.7 MB (122683473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-63.1.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4a2d4689caaf73bd66fc8f815e9608d98d52c77c0f633e8a7451b951e4ad7fdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.7 MB (200705129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436ad7cf4ae165cce24cc1dc9f6b7f1f2c31e4d1323b7c487a9448faaf57cb77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Tue, 23 May 2023 01:44:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3fff2216e0d2bfb5c1cf9eaa5494ed646c21921dae1b88da22c00dff67af15`  
		Last Modified: Tue, 23 May 2023 01:45:07 GMT  
		Size: 124.1 MB (124080383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:ad39648056b76d69619c53dd18d4aa4164e4a26b4fb1104466cf4d614c41e1fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:3e96bb61088639d6d8ceb2158cfae8d979ffe0502092c071b178175b4ddbb227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297269091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0aa9b4b68f8c9e6026e33f6b799e6da20f466f107d7973eb11b0a4e182043e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Tue, 23 May 2023 02:03:13 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017ed06ffd303ab8d53d1db147213878637053f777eb8653753bcc2631c51f7f`  
		Last Modified: Tue, 23 May 2023 02:04:46 GMT  
		Size: 218.6 MB (218601860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:4641ae6894c36dea2d891ade272dfc7c4a1d7a107a736b9654bbe2e3625b21cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191524171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf54d6f5866203f7a0fc26973af75c47b2a2d158dfd8e6bdb07aa3d3c296e635`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Tue, 23 May 2023 06:33:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b574256fc8a4e147a3ccdfb5e39fee9190b89cf93cb9496783fadeae141135`  
		Last Modified: Tue, 23 May 2023 06:34:30 GMT  
		Size: 122.7 MB (122683473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4a2d4689caaf73bd66fc8f815e9608d98d52c77c0f633e8a7451b951e4ad7fdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.7 MB (200705129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436ad7cf4ae165cce24cc1dc9f6b7f1f2c31e4d1323b7c487a9448faaf57cb77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Tue, 23 May 2023 01:44:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3fff2216e0d2bfb5c1cf9eaa5494ed646c21921dae1b88da22c00dff67af15`  
		Last Modified: Tue, 23 May 2023 01:45:07 GMT  
		Size: 124.1 MB (124080383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:ad39648056b76d69619c53dd18d4aa4164e4a26b4fb1104466cf4d614c41e1fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:3e96bb61088639d6d8ceb2158cfae8d979ffe0502092c071b178175b4ddbb227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297269091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0aa9b4b68f8c9e6026e33f6b799e6da20f466f107d7973eb11b0a4e182043e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Tue, 23 May 2023 02:03:13 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017ed06ffd303ab8d53d1db147213878637053f777eb8653753bcc2631c51f7f`  
		Last Modified: Tue, 23 May 2023 02:04:46 GMT  
		Size: 218.6 MB (218601860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4641ae6894c36dea2d891ade272dfc7c4a1d7a107a736b9654bbe2e3625b21cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191524171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf54d6f5866203f7a0fc26973af75c47b2a2d158dfd8e6bdb07aa3d3c296e635`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Tue, 23 May 2023 06:33:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b574256fc8a4e147a3ccdfb5e39fee9190b89cf93cb9496783fadeae141135`  
		Last Modified: Tue, 23 May 2023 06:34:30 GMT  
		Size: 122.7 MB (122683473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4a2d4689caaf73bd66fc8f815e9608d98d52c77c0f633e8a7451b951e4ad7fdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.7 MB (200705129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436ad7cf4ae165cce24cc1dc9f6b7f1f2c31e4d1323b7c487a9448faaf57cb77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Tue, 23 May 2023 01:44:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1edcf9e1c5be94633fa025614866d49c437322ab3cc759822645287ddb9bfd62;             SDK_ARCH="x64";;         armhf)             DART_SHA256=82c73e025efa6c4020985f85fe2b46264000295a402e1be9e787f54c17eb2590;             SDK_ARCH="arm";;         arm64)             DART_SHA256=63442bd94a4bcb043fccf9f3f22a5ca846fbb3a3933eea84dcfe8502f8f767de;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-63.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3fff2216e0d2bfb5c1cf9eaa5494ed646c21921dae1b88da22c00dff67af15`  
		Last Modified: Tue, 23 May 2023 01:45:07 GMT  
		Size: 124.1 MB (124080383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:7e51feda3a512607309bba35fc63f5504a07d704c5f45a57b5867b3f18b7acfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:cd7660c67812dc2cb66ba03879fdd078c8cb3d4b5343a516adcad01eeddbac3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296592199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3276646ebc688960f7e5b79c9b9d15f0be6ed96526c048b75069f237a7910bf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:02:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:02:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 02:02:39 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 02:02:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:02:40 GMT
WORKDIR /root
# Wed, 24 May 2023 22:19:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0ed1bd52359b583336c2a3a85fb59661d557c2ec84c51360e23f9b98a61f50ff;             SDK_ARCH="x64";;         armhf)             DART_SHA256=18ee02a7ff1117a82328410cc6f1af4e3525cddc4cf675858d499916fa3bf28e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99ebbb0f2a2f6fe0d0c2df839ca750558949d7cc88ea3315c70ff95e11fa42a9;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572b44d335a64cd955d4b4f239be22f270eae3cb4aca267178184673f806503`  
		Last Modified: Tue, 23 May 2023 02:03:34 GMT  
		Size: 45.1 MB (45102949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c8976d47ff0430694019e0a77b46eb92804bfcc3a2d3ac81ea6971476f3127`  
		Last Modified: Tue, 23 May 2023 02:03:28 GMT  
		Size: 2.2 MB (2160696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da7bba51aae91e71ac78b8e64203b88caa071b649c553191b22b63309c6be3`  
		Last Modified: Wed, 24 May 2023 22:20:19 GMT  
		Size: 217.9 MB (217924968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c2bd80683ec9105d3f92c038738cb7c9e2e354c13bb95641e11ec639d20d3742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fda967689a6e1cc06e37eaa792b82ad6c360ae38e53089b8a733e5ff89c75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:57:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498d0b6d5195e5ebb29f28dc9b4b7bc7bce8d7645d589c4b6d056f8e5ca80e46`  
		Last Modified: Fri, 02 Jun 2023 18:57:59 GMT  
		Size: 122.4 MB (122429707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3439e3dd45ed24ed1a8ffe28af318f60774424ec7300489b6426ce4b6e19d1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200456403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91983eb2e72ad604e21b324039e8ece55fadff37e4be57bacc817f2d88b841e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:43:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 01:43:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 01:43:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:43:44 GMT
WORKDIR /root
# Fri, 02 Jun 2023 18:39:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c4a2c9fb66096680bc99f687343ba9c64cc4f8a9c583c50a71ab8a63339303fc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e31ed76eedd4daf202c54d6472a4603cd60fe17d090b5e6782b18bb7b7cacee5;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d275012238a7ad416b819c74f303b152d676a82a97c3cffed01dda2915e38a0c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834f1e82c8c7a78091fc1d2da8d589129c39bb91a9f424bcca2633901f7d3fe`  
		Last Modified: Tue, 23 May 2023 01:44:25 GMT  
		Size: 45.0 MB (45011120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4b42a8d93958e89deb953ea286363c4541e1c65e8ea0f3ed34c177a7163b8`  
		Last Modified: Tue, 23 May 2023 01:44:21 GMT  
		Size: 1.6 MB (1560879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d460c04bbb531f7c61d9eb4e157157ab67946f5f221b9358793147622808301`  
		Last Modified: Fri, 02 Jun 2023 18:39:54 GMT  
		Size: 123.8 MB (123831657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
