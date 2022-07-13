<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.17`](#dart217)
-	[`dart:2.17-sdk`](#dart217-sdk)
-	[`dart:2.17.6`](#dart2176)
-	[`dart:2.17.6-sdk`](#dart2176-sdk)
-	[`dart:2.18.0-165.1.beta`](#dart2180-1651beta)
-	[`dart:2.18.0-165.1.beta-sdk`](#dart2180-1651beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:d3776dfb3591a7384de1ca45c486347ecd10ecd618a0c51c8c54b9ece97aff7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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
$ docker pull dart@sha256:d3776dfb3591a7384de1ca45c486347ecd10ecd618a0c51c8c54b9ece97aff7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
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

## `dart:2.18.0-165.1.beta`

```console
$ docker pull dart@sha256:9c624c4c2da3ca126617f7a637c45bd5351c9f149720450058d1965d558054bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:824d21c3341c7e7883eadee87bd72247f491b3100f1f051219229d9c69cbab89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280571873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896e43d677bcf9ae4405a9a67af382788ee654e5e545220b7addeffabca498f`
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
# Tue, 12 Jul 2022 02:59:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:1a03cdcdff6c02e821c28372fb42a6b0ab056254d46f0197cb71853126766c3d`  
		Last Modified: Tue, 12 Jul 2022 03:01:27 GMT  
		Size: 202.0 MB (201992407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:3cc0c5b0ae180907592b257466bd2817473d01aa36ae5ca8781f60d1d0af9f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186061132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254eb675598f178ffccbf7287070304ab935042e0a7ac8bb26ce32f3f86ccfd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:02:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2084f2890298bdd6d39eb48aca5b4df713f7ab86adf5e5a36bff7a44fb33cec3`  
		Last Modified: Tue, 12 Jul 2022 04:06:39 GMT  
		Size: 117.2 MB (117246051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:61d1241f9e82d6c79f1d1eb43be9aee12913e630e6242d910b051cf0cfa4e2f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.4 MB (195367857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbf1122b4e899a51af9f1591648dbe62639cbb1682ea40b0714d177e45b3b52`
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
# Tue, 12 Jul 2022 02:51:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:5f41c369d54d1026bcf51df7ec2f60dca011d681b0511add13c61bc8b09b0944`  
		Last Modified: Tue, 12 Jul 2022 02:52:55 GMT  
		Size: 118.8 MB (118763167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-165.1.beta-sdk`

```console
$ docker pull dart@sha256:9c624c4c2da3ca126617f7a637c45bd5351c9f149720450058d1965d558054bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:824d21c3341c7e7883eadee87bd72247f491b3100f1f051219229d9c69cbab89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280571873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896e43d677bcf9ae4405a9a67af382788ee654e5e545220b7addeffabca498f`
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
# Tue, 12 Jul 2022 02:59:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:1a03cdcdff6c02e821c28372fb42a6b0ab056254d46f0197cb71853126766c3d`  
		Last Modified: Tue, 12 Jul 2022 03:01:27 GMT  
		Size: 202.0 MB (201992407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3cc0c5b0ae180907592b257466bd2817473d01aa36ae5ca8781f60d1d0af9f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186061132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254eb675598f178ffccbf7287070304ab935042e0a7ac8bb26ce32f3f86ccfd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:02:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2084f2890298bdd6d39eb48aca5b4df713f7ab86adf5e5a36bff7a44fb33cec3`  
		Last Modified: Tue, 12 Jul 2022 04:06:39 GMT  
		Size: 117.2 MB (117246051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:61d1241f9e82d6c79f1d1eb43be9aee12913e630e6242d910b051cf0cfa4e2f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.4 MB (195367857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbf1122b4e899a51af9f1591648dbe62639cbb1682ea40b0714d177e45b3b52`
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
# Tue, 12 Jul 2022 02:51:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:5f41c369d54d1026bcf51df7ec2f60dca011d681b0511add13c61bc8b09b0944`  
		Last Modified: Tue, 12 Jul 2022 02:52:55 GMT  
		Size: 118.8 MB (118763167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:9c624c4c2da3ca126617f7a637c45bd5351c9f149720450058d1965d558054bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:824d21c3341c7e7883eadee87bd72247f491b3100f1f051219229d9c69cbab89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280571873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896e43d677bcf9ae4405a9a67af382788ee654e5e545220b7addeffabca498f`
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
# Tue, 12 Jul 2022 02:59:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:1a03cdcdff6c02e821c28372fb42a6b0ab056254d46f0197cb71853126766c3d`  
		Last Modified: Tue, 12 Jul 2022 03:01:27 GMT  
		Size: 202.0 MB (201992407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:3cc0c5b0ae180907592b257466bd2817473d01aa36ae5ca8781f60d1d0af9f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186061132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254eb675598f178ffccbf7287070304ab935042e0a7ac8bb26ce32f3f86ccfd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:02:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2084f2890298bdd6d39eb48aca5b4df713f7ab86adf5e5a36bff7a44fb33cec3`  
		Last Modified: Tue, 12 Jul 2022 04:06:39 GMT  
		Size: 117.2 MB (117246051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:61d1241f9e82d6c79f1d1eb43be9aee12913e630e6242d910b051cf0cfa4e2f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.4 MB (195367857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbf1122b4e899a51af9f1591648dbe62639cbb1682ea40b0714d177e45b3b52`
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
# Tue, 12 Jul 2022 02:51:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:5f41c369d54d1026bcf51df7ec2f60dca011d681b0511add13c61bc8b09b0944`  
		Last Modified: Tue, 12 Jul 2022 02:52:55 GMT  
		Size: 118.8 MB (118763167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:9c624c4c2da3ca126617f7a637c45bd5351c9f149720450058d1965d558054bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:824d21c3341c7e7883eadee87bd72247f491b3100f1f051219229d9c69cbab89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280571873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896e43d677bcf9ae4405a9a67af382788ee654e5e545220b7addeffabca498f`
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
# Tue, 12 Jul 2022 02:59:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:1a03cdcdff6c02e821c28372fb42a6b0ab056254d46f0197cb71853126766c3d`  
		Last Modified: Tue, 12 Jul 2022 03:01:27 GMT  
		Size: 202.0 MB (201992407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3cc0c5b0ae180907592b257466bd2817473d01aa36ae5ca8781f60d1d0af9f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186061132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254eb675598f178ffccbf7287070304ab935042e0a7ac8bb26ce32f3f86ccfd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:02:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2084f2890298bdd6d39eb48aca5b4df713f7ab86adf5e5a36bff7a44fb33cec3`  
		Last Modified: Tue, 12 Jul 2022 04:06:39 GMT  
		Size: 117.2 MB (117246051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:61d1241f9e82d6c79f1d1eb43be9aee12913e630e6242d910b051cf0cfa4e2f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.4 MB (195367857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfbf1122b4e899a51af9f1591648dbe62639cbb1682ea40b0714d177e45b3b52`
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
# Tue, 12 Jul 2022 02:51:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:5f41c369d54d1026bcf51df7ec2f60dca011d681b0511add13c61bc8b09b0944`  
		Last Modified: Tue, 12 Jul 2022 02:52:55 GMT  
		Size: 118.8 MB (118763167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
$ docker pull dart@sha256:53332996ddcdd1f45a09a71d1ec9fa0fb1c837aa7c8bdcc88bb8f6d097f393bb
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
$ docker pull dart@sha256:d6828fadccaceccc8072eac73568ce163ac21126316f3282b1154709058446ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184059360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f8268d479dadb534ab5c992fd0faa90367eff3026b97dd1d5d5944c6e00898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:00:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:00:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 04:00:59 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 04:00:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 04:00:59 GMT
WORKDIR /root
# Tue, 12 Jul 2022 04:01:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0052467a23ec8d46523be0f29263881444e0da3228860eb6b69de0859aca2459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=00e855429cd7345a56235a7b216967d23c22d0c1a0417249c4323b1cbfe9af62;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0482ba914c7e9befc67d1ff0057bfcae354d6cfeb0d4716f1ff44623089a2688;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4316fd66656dd89ade0257dac476c6229bb11452333cb88904df00760175d4`  
		Last Modified: Tue, 12 Jul 2022 04:03:48 GMT  
		Size: 41.0 MB (40966440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de87ab189edecdb2c70e7ebd1274844a743ed886eace795c9d9eeef8a499e64`  
		Last Modified: Tue, 12 Jul 2022 04:03:24 GMT  
		Size: 1.3 MB (1288082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ca16399f4184877ecbc3567a5c1144991fcdf3c3d2824971c2b8c55363cd5f`  
		Last Modified: Tue, 12 Jul 2022 04:04:38 GMT  
		Size: 115.2 MB (115244279 bytes)  
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
