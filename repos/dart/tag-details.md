<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:3`](#dart3)
-	[`dart:3-sdk`](#dart3-sdk)
-	[`dart:3.0`](#dart30)
-	[`dart:3.0-sdk`](#dart30-sdk)
-	[`dart:3.0.6`](#dart306)
-	[`dart:3.0.6-sdk`](#dart306-sdk)
-	[`dart:3.1.0-262.1.beta`](#dart310-2621beta)
-	[`dart:3.1.0-262.1.beta-sdk`](#dart310-2621beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:3`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3-sdk`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0-sdk`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.6`

```console
$ docker pull dart@sha256:497b8d348a967b4e9f1f6983e29b988cac22cfcd9672bb0233a31db4c8a6db4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm variant v7

### `dart:3.0.6` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.6` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.6-sdk`

```console
$ docker pull dart@sha256:497b8d348a967b4e9f1f6983e29b988cac22cfcd9672bb0233a31db4c8a6db4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm variant v7

### `dart:3.0.6-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.6-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-262.1.beta`

```console
$ docker pull dart@sha256:4d91faed427378b6726ce81080a3dbdfc64cc2e2bb044a30477f8f91f6c545d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm variant v7

### `dart:3.1.0-262.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:7de21dc69501dec5cc65b72995f69e0d3785678b6a102b47dc756d51aaedc1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291214954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e3a03051a15482dce93c734f198ed1c1b461e66008558453470ff933f14671`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4bf41bc433dff3a0feea5f81353004d7122ea407621a7c32444b73ade91f43`  
		Last Modified: Wed, 12 Jul 2023 19:21:37 GMT  
		Size: 212.5 MB (212535272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-262.1.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:d8674470f340ba018c9365c7fa3c38a693e68706e08e2d82ac01d3bd45a86554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182226939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3612b19269850facfac31d6f99ea35f706099d80e659508520ecdb83249ec9ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25e3df59c73e27f1cd086ee90431af14b7ccd7f17ffefdca73ad1895221e30`  
		Last Modified: Wed, 12 Jul 2023 18:59:05 GMT  
		Size: 113.4 MB (113372111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-262.1.beta-sdk`

```console
$ docker pull dart@sha256:4d91faed427378b6726ce81080a3dbdfc64cc2e2bb044a30477f8f91f6c545d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm variant v7

### `dart:3.1.0-262.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7de21dc69501dec5cc65b72995f69e0d3785678b6a102b47dc756d51aaedc1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291214954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e3a03051a15482dce93c734f198ed1c1b461e66008558453470ff933f14671`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4bf41bc433dff3a0feea5f81353004d7122ea407621a7c32444b73ade91f43`  
		Last Modified: Wed, 12 Jul 2023 19:21:37 GMT  
		Size: 212.5 MB (212535272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-262.1.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:d8674470f340ba018c9365c7fa3c38a693e68706e08e2d82ac01d3bd45a86554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182226939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3612b19269850facfac31d6f99ea35f706099d80e659508520ecdb83249ec9ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25e3df59c73e27f1cd086ee90431af14b7ccd7f17ffefdca73ad1895221e30`  
		Last Modified: Wed, 12 Jul 2023 18:59:05 GMT  
		Size: 113.4 MB (113372111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:2088316e4ea8af18e38ab2f837cd6ec023d284c6b796e1bda222499908aa7401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:7de21dc69501dec5cc65b72995f69e0d3785678b6a102b47dc756d51aaedc1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291214954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e3a03051a15482dce93c734f198ed1c1b461e66008558453470ff933f14671`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4bf41bc433dff3a0feea5f81353004d7122ea407621a7c32444b73ade91f43`  
		Last Modified: Wed, 12 Jul 2023 19:21:37 GMT  
		Size: 212.5 MB (212535272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:d8674470f340ba018c9365c7fa3c38a693e68706e08e2d82ac01d3bd45a86554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182226939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3612b19269850facfac31d6f99ea35f706099d80e659508520ecdb83249ec9ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25e3df59c73e27f1cd086ee90431af14b7ccd7f17ffefdca73ad1895221e30`  
		Last Modified: Wed, 12 Jul 2023 18:59:05 GMT  
		Size: 113.4 MB (113372111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d938f6d32e20408c71a17f2b399f38c07d7029826137a29ed3bfa625fb379c0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187987542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e29190e750d7d752e8061dbe44fc5f72d5c7b3a1980f16bc23609e97f31d100`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:28:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fe06f5c812cec123a41670ea391f3154962a4922ac77f34dd0366c3b4eb4a5`  
		Last Modified: Tue, 04 Jul 2023 06:29:16 GMT  
		Size: 111.4 MB (111351794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:2088316e4ea8af18e38ab2f837cd6ec023d284c6b796e1bda222499908aa7401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7de21dc69501dec5cc65b72995f69e0d3785678b6a102b47dc756d51aaedc1a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291214954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e3a03051a15482dce93c734f198ed1c1b461e66008558453470ff933f14671`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4bf41bc433dff3a0feea5f81353004d7122ea407621a7c32444b73ade91f43`  
		Last Modified: Wed, 12 Jul 2023 19:21:37 GMT  
		Size: 212.5 MB (212535272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:d8674470f340ba018c9365c7fa3c38a693e68706e08e2d82ac01d3bd45a86554
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182226939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3612b19269850facfac31d6f99ea35f706099d80e659508520ecdb83249ec9ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=18f959e4361833fac9421bfba51341df1141bfff16c1261852de7d87d883f2ea;             SDK_ARCH="x64";;         armhf)             DART_SHA256=8a9e840c238aa7a5c16f47d92e7edb8883962a08e32bf474de9a674182f21619;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3f54e64b2974c232f4580c2103ace293b6f5070976f68632629f392843016779;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25e3df59c73e27f1cd086ee90431af14b7ccd7f17ffefdca73ad1895221e30`  
		Last Modified: Wed, 12 Jul 2023 18:59:05 GMT  
		Size: 113.4 MB (113372111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d938f6d32e20408c71a17f2b399f38c07d7029826137a29ed3bfa625fb379c0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187987542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e29190e750d7d752e8061dbe44fc5f72d5c7b3a1980f16bc23609e97f31d100`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:28:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fe06f5c812cec123a41670ea391f3154962a4922ac77f34dd0366c3b4eb4a5`  
		Last Modified: Tue, 04 Jul 2023 06:29:16 GMT  
		Size: 111.4 MB (111351794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:c7bfb7f26043804bf496c2943719295766409bd6aaffd57d33809178d024be0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e87f2c9ec63a2b02aef6f0be80080f4cb7ddd09c56857674163298283c6aaa4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200467849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a096055c3ec8cc7632ae8eb40986bdae9f3680117a13f600d1991b8374c88b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Tue, 04 Jul 2023 06:27:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=05fba372d64932dffce90bbd45116b76806bf9adc6203967b56faf5c64b2b66c;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ed151fd396522c09c41820e627eea8a72da973f7e0aeef8e8099c914b7fde2c1;             SDK_ARCH="arm";;         arm64)             DART_SHA256=667b79593444cbe222a33c137ca943dced7a21ff2d61b8862f3b49e648c20533;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba903f845f28ef562c865f518503ce19ad43c0900e4d8dbc6d6bd04da7e8ac`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 123.8 MB (123832101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
