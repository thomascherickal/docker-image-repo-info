<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.17`](#dart217)
-	[`dart:2.17-sdk`](#dart217-sdk)
-	[`dart:2.17.6`](#dart2176)
-	[`dart:2.17.6-sdk`](#dart2176-sdk)
-	[`dart:2.18.0-271.4.beta`](#dart2180-2714beta)
-	[`dart:2.18.0-271.4.beta-sdk`](#dart2180-2714beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17-sdk`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17-sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.6`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.6` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.6` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.6` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.6-sdk`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.6-sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.6-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.6-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-271.4.beta`

```console
$ docker pull dart@sha256:ca8646253f1ef4ca8a54f9ce2e220b908fa605ab25a4925b0cb5720dcfc7b7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-271.4.beta` - linux; amd64

```console
$ docker pull dart@sha256:0cd79e8cb106e85c25d7ac135c2f261a2d6a09d38f9d5d15594ca11a1fa4a1b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271864253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b978ed4e4d65ba937ca915ce422747dae6ed2c1e56eea679655765e30f3e97c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 27 Jul 2022 19:21:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf996220ede3ac03d5fa3fbb391a1f64d2f7cf251592d08763ca9209a34fc0e`  
		Last Modified: Wed, 27 Jul 2022 19:22:31 GMT  
		Size: 193.3 MB (193284787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-271.4.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:de577152a3e8ab4d73d0a29c399964070db77a52228e503f7ece1a7bdad69089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180555692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bbbc50aca87f45bc77c9b8c1c39a56aee12640a05939506b52a2c71c17654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12c255e1b735986ba8bfc29f84f62379e339eaac1bef3973b36019cdd777db7`  
		Last Modified: Thu, 28 Jul 2022 14:11:47 GMT  
		Size: 111.7 MB (111740696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-271.4.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3090bc105c13a2070c7a1a1714e60460e1fda2a2a83623d01dcd95de796011ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189689387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d03200eb1977283d227ca9e2e9a3ec882a685902fd972f11403c4b923cb0f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 27 Jul 2022 20:22:30 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c4f72e67c053388232de60333c3e92616078d2e28a90d7235fc8caa268ee`  
		Last Modified: Wed, 27 Jul 2022 20:23:28 GMT  
		Size: 113.1 MB (113084697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-271.4.beta-sdk`

```console
$ docker pull dart@sha256:ca8646253f1ef4ca8a54f9ce2e220b908fa605ab25a4925b0cb5720dcfc7b7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-271.4.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:0cd79e8cb106e85c25d7ac135c2f261a2d6a09d38f9d5d15594ca11a1fa4a1b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271864253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b978ed4e4d65ba937ca915ce422747dae6ed2c1e56eea679655765e30f3e97c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 27 Jul 2022 19:21:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf996220ede3ac03d5fa3fbb391a1f64d2f7cf251592d08763ca9209a34fc0e`  
		Last Modified: Wed, 27 Jul 2022 19:22:31 GMT  
		Size: 193.3 MB (193284787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-271.4.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:de577152a3e8ab4d73d0a29c399964070db77a52228e503f7ece1a7bdad69089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180555692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bbbc50aca87f45bc77c9b8c1c39a56aee12640a05939506b52a2c71c17654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12c255e1b735986ba8bfc29f84f62379e339eaac1bef3973b36019cdd777db7`  
		Last Modified: Thu, 28 Jul 2022 14:11:47 GMT  
		Size: 111.7 MB (111740696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-271.4.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3090bc105c13a2070c7a1a1714e60460e1fda2a2a83623d01dcd95de796011ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189689387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d03200eb1977283d227ca9e2e9a3ec882a685902fd972f11403c4b923cb0f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 27 Jul 2022 20:22:30 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c4f72e67c053388232de60333c3e92616078d2e28a90d7235fc8caa268ee`  
		Last Modified: Wed, 27 Jul 2022 20:23:28 GMT  
		Size: 113.1 MB (113084697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:ca8646253f1ef4ca8a54f9ce2e220b908fa605ab25a4925b0cb5720dcfc7b7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:0cd79e8cb106e85c25d7ac135c2f261a2d6a09d38f9d5d15594ca11a1fa4a1b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271864253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b978ed4e4d65ba937ca915ce422747dae6ed2c1e56eea679655765e30f3e97c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 27 Jul 2022 19:21:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf996220ede3ac03d5fa3fbb391a1f64d2f7cf251592d08763ca9209a34fc0e`  
		Last Modified: Wed, 27 Jul 2022 19:22:31 GMT  
		Size: 193.3 MB (193284787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:de577152a3e8ab4d73d0a29c399964070db77a52228e503f7ece1a7bdad69089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180555692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bbbc50aca87f45bc77c9b8c1c39a56aee12640a05939506b52a2c71c17654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12c255e1b735986ba8bfc29f84f62379e339eaac1bef3973b36019cdd777db7`  
		Last Modified: Thu, 28 Jul 2022 14:11:47 GMT  
		Size: 111.7 MB (111740696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3090bc105c13a2070c7a1a1714e60460e1fda2a2a83623d01dcd95de796011ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189689387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d03200eb1977283d227ca9e2e9a3ec882a685902fd972f11403c4b923cb0f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 27 Jul 2022 20:22:30 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c4f72e67c053388232de60333c3e92616078d2e28a90d7235fc8caa268ee`  
		Last Modified: Wed, 27 Jul 2022 20:23:28 GMT  
		Size: 113.1 MB (113084697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:ca8646253f1ef4ca8a54f9ce2e220b908fa605ab25a4925b0cb5720dcfc7b7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:0cd79e8cb106e85c25d7ac135c2f261a2d6a09d38f9d5d15594ca11a1fa4a1b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271864253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b978ed4e4d65ba937ca915ce422747dae6ed2c1e56eea679655765e30f3e97c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 27 Jul 2022 19:21:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf996220ede3ac03d5fa3fbb391a1f64d2f7cf251592d08763ca9209a34fc0e`  
		Last Modified: Wed, 27 Jul 2022 19:22:31 GMT  
		Size: 193.3 MB (193284787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:de577152a3e8ab4d73d0a29c399964070db77a52228e503f7ece1a7bdad69089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180555692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bbbc50aca87f45bc77c9b8c1c39a56aee12640a05939506b52a2c71c17654`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12c255e1b735986ba8bfc29f84f62379e339eaac1bef3973b36019cdd777db7`  
		Last Modified: Thu, 28 Jul 2022 14:11:47 GMT  
		Size: 111.7 MB (111740696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3090bc105c13a2070c7a1a1714e60460e1fda2a2a83623d01dcd95de796011ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189689387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d03200eb1977283d227ca9e2e9a3ec882a685902fd972f11403c4b923cb0f0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 27 Jul 2022 20:22:30 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d058dfd1487e7f8344b812f00ef4ee9dec455743a6c3c222c07c53083cbcd1e4;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10a0d64eaa8e0ffbb229252ae08359a27af97a72026867e756c7c68a992d5544;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2c280eded97e7f42df56302ac83f910f1b0c059817870d953e5b356add0156a4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-271.4.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c4f72e67c053388232de60333c3e92616078d2e28a90d7235fc8caa268ee`  
		Last Modified: Wed, 27 Jul 2022 20:23:28 GMT  
		Size: 113.1 MB (113084697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:182556e4cafe3969e5227cdc685bbc04543a60b58b628fbbeb62f8d1a3509ac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:382901c556f72809e7438d2515f1629181aff44f144c1aae995bc4653b2b0d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193339198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476fafcb97db71bc6a5d30b05842fc1263518d3c98bc6cd6658137070ff2917c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:50:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:50:26 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:50:27 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:50:28 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:40:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e246275131a2c58b895f382305d66ca2a62c8a433f275f1af8487179ec55d8`  
		Last Modified: Tue, 12 Jul 2022 02:51:50 GMT  
		Size: 45.0 MB (44993733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21622692fc0cf8e1b2d476c3dd08928da6df9f71f634746ca0362125b8b58dd`  
		Last Modified: Tue, 12 Jul 2022 02:51:43 GMT  
		Size: 1.6 MB (1556731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebb73a77d2aab991e0e4eaf35d599a85f32d588009c5af017e2e404f9a161d`  
		Last Modified: Wed, 13 Jul 2022 19:41:03 GMT  
		Size: 116.7 MB (116734508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
