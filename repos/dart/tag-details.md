<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.14`](#dart214)
-	[`dart:2.14-sdk`](#dart214-sdk)
-	[`dart:2.14.4`](#dart2144)
-	[`dart:2.14.4-sdk`](#dart2144-sdk)
-	[`dart:2.15.0-268.18.beta`](#dart2150-26818beta)
-	[`dart:2.15.0-268.18.beta-sdk`](#dart2150-26818beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14-sdk`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14-sdk` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.4`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14.4` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.4-sdk`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14.4-sdk` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-268.18.beta`

```console
$ docker pull dart@sha256:8093f51bf091845bc1700b358842b5002f207e87fbaef274cf49a4a4ca9e4a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `dart:2.15.0-268.18.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3ac5ffc7bbcd8cc42cf3c741e0c4aee123c35a4c54ae497f5990121d28491b4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193757962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adb7ec516e2de9624da0e3cd26604bf563808d46cb9e582078aca2385251422`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Thu, 18 Nov 2021 08:26:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c93c72123f27836e9a6131a5e24b46fede7570f0388b5c9afef8f71232fdaf84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6525d9b92bed7dde3576d59333c8367b92f1b4a6e6e005918717728c9451fe89;             SDK_ARCH="arm";;         arm64)             DART_SHA256=aec5056aa84bf8813d75f392e1659646a868bbb944ff1d3fc5d95282b987f771;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.18.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd78e5947d73fe449c2843643e6181f582a680598b123d482f743e4e229145`  
		Last Modified: Thu, 18 Nov 2021 08:27:33 GMT  
		Size: 116.6 MB (116563930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-268.18.beta-sdk`

```console
$ docker pull dart@sha256:8093f51bf091845bc1700b358842b5002f207e87fbaef274cf49a4a4ca9e4a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `dart:2.15.0-268.18.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3ac5ffc7bbcd8cc42cf3c741e0c4aee123c35a4c54ae497f5990121d28491b4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193757962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adb7ec516e2de9624da0e3cd26604bf563808d46cb9e582078aca2385251422`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Thu, 18 Nov 2021 08:26:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c93c72123f27836e9a6131a5e24b46fede7570f0388b5c9afef8f71232fdaf84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6525d9b92bed7dde3576d59333c8367b92f1b4a6e6e005918717728c9451fe89;             SDK_ARCH="arm";;         arm64)             DART_SHA256=aec5056aa84bf8813d75f392e1659646a868bbb944ff1d3fc5d95282b987f771;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.18.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd78e5947d73fe449c2843643e6181f582a680598b123d482f743e4e229145`  
		Last Modified: Thu, 18 Nov 2021 08:27:33 GMT  
		Size: 116.6 MB (116563930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:c4be44c6849331fd8723a068ddfac93de964adbc781732c332b99b30d9a1a437
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:c55eb18ea018419674fccd8b57cc89e499feb9703e92b965044b4fdf59a7441b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.3 MB (276285469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714f87662781de083a3fa981d2e3571022e6d9cbcd7e0145803d8e73b215b7cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:49 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aa1a5004334ae4070b59d1ef14cfeb02999f1ece827bb77445e9dbbfeaf6ef`  
		Last Modified: Wed, 17 Nov 2021 03:35:57 GMT  
		Size: 197.2 MB (197189178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:9ca4a0933ae0df4169c3f6b2e55c81464ffee607bb211dacab928df748727445
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183694739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0edefddfccc042daf4aaf24e53b2df2c21c019ab046e6110d9a1be6b4f4a8c2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606672ac20c822a2f7bf089cc54eb5818cdf201d2596759cc93c4f7f0beb61d0`  
		Last Modified: Wed, 17 Nov 2021 03:24:37 GMT  
		Size: 115.2 MB (115185017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3ac5ffc7bbcd8cc42cf3c741e0c4aee123c35a4c54ae497f5990121d28491b4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193757962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adb7ec516e2de9624da0e3cd26604bf563808d46cb9e582078aca2385251422`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Thu, 18 Nov 2021 08:26:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c93c72123f27836e9a6131a5e24b46fede7570f0388b5c9afef8f71232fdaf84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6525d9b92bed7dde3576d59333c8367b92f1b4a6e6e005918717728c9451fe89;             SDK_ARCH="arm";;         arm64)             DART_SHA256=aec5056aa84bf8813d75f392e1659646a868bbb944ff1d3fc5d95282b987f771;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.18.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd78e5947d73fe449c2843643e6181f582a680598b123d482f743e4e229145`  
		Last Modified: Thu, 18 Nov 2021 08:27:33 GMT  
		Size: 116.6 MB (116563930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:c4be44c6849331fd8723a068ddfac93de964adbc781732c332b99b30d9a1a437
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:c55eb18ea018419674fccd8b57cc89e499feb9703e92b965044b4fdf59a7441b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.3 MB (276285469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714f87662781de083a3fa981d2e3571022e6d9cbcd7e0145803d8e73b215b7cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:49 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aa1a5004334ae4070b59d1ef14cfeb02999f1ece827bb77445e9dbbfeaf6ef`  
		Last Modified: Wed, 17 Nov 2021 03:35:57 GMT  
		Size: 197.2 MB (197189178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9ca4a0933ae0df4169c3f6b2e55c81464ffee607bb211dacab928df748727445
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183694739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0edefddfccc042daf4aaf24e53b2df2c21c019ab046e6110d9a1be6b4f4a8c2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:20:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606672ac20c822a2f7bf089cc54eb5818cdf201d2596759cc93c4f7f0beb61d0`  
		Last Modified: Wed, 17 Nov 2021 03:24:37 GMT  
		Size: 115.2 MB (115185017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3ac5ffc7bbcd8cc42cf3c741e0c4aee123c35a4c54ae497f5990121d28491b4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193757962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adb7ec516e2de9624da0e3cd26604bf563808d46cb9e582078aca2385251422`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Thu, 18 Nov 2021 08:26:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c93c72123f27836e9a6131a5e24b46fede7570f0388b5c9afef8f71232fdaf84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6525d9b92bed7dde3576d59333c8367b92f1b4a6e6e005918717728c9451fe89;             SDK_ARCH="arm";;         arm64)             DART_SHA256=aec5056aa84bf8813d75f392e1659646a868bbb944ff1d3fc5d95282b987f771;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.18.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd78e5947d73fe449c2843643e6181f582a680598b123d482f743e4e229145`  
		Last Modified: Thu, 18 Nov 2021 08:27:33 GMT  
		Size: 116.6 MB (116563930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:17faa8d1476c27ad67ad0d85c0f33e34406fa55003e11bf62528bf5aa21fb782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:45b14580569670f010a924b59a11ebe18f3ae78b3a09815e959a38f18f04dcf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289082141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a0f2042b77733dce1ec8b69af98166f5b3d39875c3afd70ca01a37ae88b67f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:33:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:33:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:33:09 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:33:09 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:33:09 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:33:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a8a7220d40c196ed357398ceefc39cc9cbf1c7365a38e58a5ff7dd0c729a0`  
		Last Modified: Wed, 17 Nov 2021 03:34:26 GMT  
		Size: 49.6 MB (49583477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820270e6cdbd4bed05cb38a40c37c3725678f2c73b20dd28d033f7b98f98543`  
		Last Modified: Wed, 17 Nov 2021 03:34:15 GMT  
		Size: 2.4 MB (2359139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2216bfcb43baa7a8cbc9248c2af577befb9be01dd132f16048dfa8e315f3d0`  
		Last Modified: Wed, 17 Nov 2021 03:34:53 GMT  
		Size: 210.0 MB (209985850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:3475edc2507a76e75e8a334f20290cca2923a3eb95e7817ed9a53834ac1fe001
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190278642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d41a3a092a7f0e205bac990ea4456a87ecad69a630fe53d62c3f257e8bc87a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:18:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 03:19:01 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 03:19:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 03:19:02 GMT
WORKDIR /root
# Wed, 17 Nov 2021 03:19:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d48b90badaa124b4a6d60d55dd6577d96988edfe844fb29c5f74a11282403b`  
		Last Modified: Wed, 17 Nov 2021 03:21:46 GMT  
		Size: 44.4 MB (44399460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7607ca2febaa8b44687332fe82feec9cced18767dbf43e991ea9c00a4a4385`  
		Last Modified: Wed, 17 Nov 2021 03:21:21 GMT  
		Size: 1.4 MB (1355903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b7910a47db93034e43842e61b9baddee7d96be1c5c30eb1c9d16680953ddd`  
		Last Modified: Wed, 17 Nov 2021 03:22:39 GMT  
		Size: 121.8 MB (121768920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8bf63eeda10f9cffb5e22f73797ad431ef65d9443f745dab933b5e3594a4fc8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200018432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d1731b5cd97af6939b1d4e935af8241a1c73717c6b3c18576cc8c7cb632bf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:15:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:15:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 17 Nov 2021 10:15:33 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 17 Nov 2021 10:15:34 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 10:15:35 GMT
WORKDIR /root
# Wed, 17 Nov 2021 10:15:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2657e962e18ef870db370c74562b339e217153aec72566fb3b666fd3c37175`  
		Last Modified: Wed, 17 Nov 2021 10:16:49 GMT  
		Size: 49.6 MB (49638991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2844b14d112904a7db4d890cdcaa3f1014a23307ed4bc8fc31139df030bd65`  
		Last Modified: Wed, 17 Nov 2021 10:16:43 GMT  
		Size: 1.6 MB (1631924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1338b7b40e372b19b7f0ae1c87fa656900709c43f658f09978b97889966e7`  
		Last Modified: Wed, 17 Nov 2021 10:17:00 GMT  
		Size: 122.8 MB (122824400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
