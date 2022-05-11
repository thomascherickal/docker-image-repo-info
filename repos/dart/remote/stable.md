## `dart:stable`

```console
$ docker pull dart@sha256:9c86b911406bbb6aa799089cffd2c70b22ba92eed3880938c04ad8fa79833bcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:f6dbc121c9cf59ba8e7a21b9ef52378f1c720b3fe09f13f2edd1e6acf5a1acd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279617255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c0269f02bc8073a7f862226fe81b1bbb38f9017f7747e73d9d25201fb7a037`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:07:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:07:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 May 2022 02:07:40 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 May 2022 02:07:41 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 02:07:41 GMT
WORKDIR /root
# Wed, 11 May 2022 02:07:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e018694dc31933ae0740198514b84926070fb8960619b94a547bd6b8176089`  
		Last Modified: Wed, 11 May 2022 02:08:38 GMT  
		Size: 45.1 MB (45073059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6825a70fa3a955287cb5534a3ed5e22826ea58c6775422fa6173b0692951ad4b`  
		Last Modified: Wed, 11 May 2022 02:08:31 GMT  
		Size: 2.1 MB (2139537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff3033c8a360721a315c0e469ccf453aad5d749a557036ddf5a2a53e885d21c`  
		Last Modified: Wed, 11 May 2022 02:09:00 GMT  
		Size: 201.0 MB (201025183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:4bfd523db407121be7979185f524d71e2b7b2a1917bb4b01471365e63bcc72d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7887d8d7e881f2b7de8838b9ad483dd1c260c53c6e2a083ad369fff7a5cd0d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:06:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:06:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 May 2022 04:06:15 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 May 2022 04:06:16 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 04:06:16 GMT
WORKDIR /root
# Wed, 11 May 2022 04:06:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3a9fda181c5ab34eadfaa2e3cb43e5927f454b816b486d9d46966b36f00169`  
		Last Modified: Wed, 11 May 2022 04:08:53 GMT  
		Size: 41.0 MB (40966751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0614044a348b11e843b72ffba5071df750d80d83c220b5818815b1a54dd391d`  
		Last Modified: Wed, 11 May 2022 04:08:29 GMT  
		Size: 1.3 MB (1288076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bd542dbb90507734ca1baa4ffe54bfba8fc437005e76a7a61ff4f0738bbc3d`  
		Last Modified: Wed, 11 May 2022 04:09:43 GMT  
		Size: 118.2 MB (118189580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:87ef95bf5edd916a421f9a939f2a6c972426248564be666863f158ebe8707135
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7f1fcad43cafeed50f09effa5443a141eef295e5fc579e3e773fbec3a94c76`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:12:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:12:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 May 2022 14:12:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 May 2022 14:12:05 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:12:06 GMT
WORKDIR /root
# Wed, 11 May 2022 14:12:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538f75f7492080dc6c80ccc3b0a9324f82c715a990e4f527832dda7b716be2b9`  
		Last Modified: Wed, 11 May 2022 14:13:17 GMT  
		Size: 44.8 MB (44789413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de512492e0fc65df4789b2cd72bcb5c1583d1bd6b97f88c5a3cb37a23d3cbd92`  
		Last Modified: Wed, 11 May 2022 14:13:11 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472461baf9528ea5c8db54edb14488e00a99fbabfddb829031e4f052c9166d63`  
		Last Modified: Wed, 11 May 2022 14:13:28 GMT  
		Size: 119.7 MB (119700892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
