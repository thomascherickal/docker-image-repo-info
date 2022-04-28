<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.16`](#dart216)
-	[`dart:2.16-sdk`](#dart216-sdk)
-	[`dart:2.16.2`](#dart2162)
-	[`dart:2.16.2-sdk`](#dart2162-sdk)
-	[`dart:2.17.0-266.7.beta`](#dart2170-2667beta)
-	[`dart:2.17.0-266.7.beta-sdk`](#dart2170-2667beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16-sdk`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.2`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.2` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.2-sdk`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.0-266.7.beta`

```console
$ docker pull dart@sha256:f9134bafd94743b104c40c7da29d70acae59781943da40ad86778f5237bd98a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.0-266.7.beta` - linux; amd64

```console
$ docker pull dart@sha256:63ff60883736b48f179d795bbe555054a131ed0bc9b3e67185cd860bc3bf1e4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275782376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efef526ddfc1e4ad2a0fe3402680bdd4812a0f33f871bd7a4ae89f4f93a5c929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 27 Apr 2022 20:43:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146e45ad8037b6f4f4b6b685d0807336bec2dbb6cd45402357048e6a93ffa33a`  
		Last Modified: Wed, 27 Apr 2022 20:44:50 GMT  
		Size: 197.2 MB (197191152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-266.7.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:402ebf4f01f9d9d2c080437555421c268d1314e2713e2143e63e7871aa160626
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b96f06f52843bc86bba2132abc719d1b7dbe0b0bde3cd3ee48ffb75b00beb3d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 27 Apr 2022 21:49:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5b143a43b3eb407c55c755721126d2fa04d31e8c8c306b5ea9a2837bfeebf6`  
		Last Modified: Wed, 27 Apr 2022 21:51:46 GMT  
		Size: 115.2 MB (115243690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-266.7.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:ef899551a338c926fbddcfaf905d371d9a25921d2f6cd77fe3d4f73286b8c242
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b49c6c3d93d3e9e6068e9a8e19ff9d419370fc1fd5158a0ef65adba8f34397`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 27 Apr 2022 23:13:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00103ce4c2079dabbd48499e8fca4c38f564d2b5603f6d57ee3d47ab04623f7d`  
		Last Modified: Wed, 27 Apr 2022 23:14:44 GMT  
		Size: 116.7 MB (116740426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.0-266.7.beta-sdk`

```console
$ docker pull dart@sha256:f9134bafd94743b104c40c7da29d70acae59781943da40ad86778f5237bd98a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.0-266.7.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:63ff60883736b48f179d795bbe555054a131ed0bc9b3e67185cd860bc3bf1e4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275782376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efef526ddfc1e4ad2a0fe3402680bdd4812a0f33f871bd7a4ae89f4f93a5c929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 27 Apr 2022 20:43:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146e45ad8037b6f4f4b6b685d0807336bec2dbb6cd45402357048e6a93ffa33a`  
		Last Modified: Wed, 27 Apr 2022 20:44:50 GMT  
		Size: 197.2 MB (197191152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-266.7.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:402ebf4f01f9d9d2c080437555421c268d1314e2713e2143e63e7871aa160626
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b96f06f52843bc86bba2132abc719d1b7dbe0b0bde3cd3ee48ffb75b00beb3d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 27 Apr 2022 21:49:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5b143a43b3eb407c55c755721126d2fa04d31e8c8c306b5ea9a2837bfeebf6`  
		Last Modified: Wed, 27 Apr 2022 21:51:46 GMT  
		Size: 115.2 MB (115243690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-266.7.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:ef899551a338c926fbddcfaf905d371d9a25921d2f6cd77fe3d4f73286b8c242
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b49c6c3d93d3e9e6068e9a8e19ff9d419370fc1fd5158a0ef65adba8f34397`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 27 Apr 2022 23:13:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00103ce4c2079dabbd48499e8fca4c38f564d2b5603f6d57ee3d47ab04623f7d`  
		Last Modified: Wed, 27 Apr 2022 23:14:44 GMT  
		Size: 116.7 MB (116740426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:f9134bafd94743b104c40c7da29d70acae59781943da40ad86778f5237bd98a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:63ff60883736b48f179d795bbe555054a131ed0bc9b3e67185cd860bc3bf1e4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275782376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efef526ddfc1e4ad2a0fe3402680bdd4812a0f33f871bd7a4ae89f4f93a5c929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 27 Apr 2022 20:43:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146e45ad8037b6f4f4b6b685d0807336bec2dbb6cd45402357048e6a93ffa33a`  
		Last Modified: Wed, 27 Apr 2022 20:44:50 GMT  
		Size: 197.2 MB (197191152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:402ebf4f01f9d9d2c080437555421c268d1314e2713e2143e63e7871aa160626
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b96f06f52843bc86bba2132abc719d1b7dbe0b0bde3cd3ee48ffb75b00beb3d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 27 Apr 2022 21:49:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5b143a43b3eb407c55c755721126d2fa04d31e8c8c306b5ea9a2837bfeebf6`  
		Last Modified: Wed, 27 Apr 2022 21:51:46 GMT  
		Size: 115.2 MB (115243690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:ef899551a338c926fbddcfaf905d371d9a25921d2f6cd77fe3d4f73286b8c242
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b49c6c3d93d3e9e6068e9a8e19ff9d419370fc1fd5158a0ef65adba8f34397`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 27 Apr 2022 23:13:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00103ce4c2079dabbd48499e8fca4c38f564d2b5603f6d57ee3d47ab04623f7d`  
		Last Modified: Wed, 27 Apr 2022 23:14:44 GMT  
		Size: 116.7 MB (116740426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:f9134bafd94743b104c40c7da29d70acae59781943da40ad86778f5237bd98a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:63ff60883736b48f179d795bbe555054a131ed0bc9b3e67185cd860bc3bf1e4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275782376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efef526ddfc1e4ad2a0fe3402680bdd4812a0f33f871bd7a4ae89f4f93a5c929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 27 Apr 2022 20:43:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146e45ad8037b6f4f4b6b685d0807336bec2dbb6cd45402357048e6a93ffa33a`  
		Last Modified: Wed, 27 Apr 2022 20:44:50 GMT  
		Size: 197.2 MB (197191152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:402ebf4f01f9d9d2c080437555421c268d1314e2713e2143e63e7871aa160626
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b96f06f52843bc86bba2132abc719d1b7dbe0b0bde3cd3ee48ffb75b00beb3d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 27 Apr 2022 21:49:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5b143a43b3eb407c55c755721126d2fa04d31e8c8c306b5ea9a2837bfeebf6`  
		Last Modified: Wed, 27 Apr 2022 21:51:46 GMT  
		Size: 115.2 MB (115243690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:ef899551a338c926fbddcfaf905d371d9a25921d2f6cd77fe3d4f73286b8c242
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b49c6c3d93d3e9e6068e9a8e19ff9d419370fc1fd5158a0ef65adba8f34397`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 27 Apr 2022 23:13:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00103ce4c2079dabbd48499e8fca4c38f564d2b5603f6d57ee3d47ab04623f7d`  
		Last Modified: Wed, 27 Apr 2022 23:14:44 GMT  
		Size: 116.7 MB (116740426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:a4b1ceb885689bfe2ebf79b1e0c496a960c2479f2f45f1311a01c9d08c6ea21a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a64fb365f140176f27cc62e13e68b3147e328fa5be382ec96a17df9a0fe6fbd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cdaffab48fd71126198a12c956f04d1668bba959b03905bb05eb64279228d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:13:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7677d65966f1f535ea55ade08a09938fc64cfcaff768606f6b328202618ccc`  
		Last Modified: Wed, 20 Apr 2022 07:14:56 GMT  
		Size: 201.0 MB (201025181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:18025d829f42f00567d58ac7c0dc3519748daa4eccf5b33677170b25e623e9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187020092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ddbbbeea1a41226d3558b0248ccdef2bf86ac27a6a5e89850485dc35b4447d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510d216fa83941069190620a102b2af58597abf4cdea8b1b81bcb3f7ef0059a`  
		Last Modified: Wed, 20 Apr 2022 20:54:12 GMT  
		Size: 118.2 MB (118189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7c9ee6bb9517f37eb5b51ecae1c5c98b35708905c7ebbf2481a47b0e9658f4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196112590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3956443f2ed3a9d41a2ba140c58c0cce3c4d7f3376faa7ac72e40693423c3fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694edfb438beb9500e0c762064ae85bdecf569d8c0c8118265704363f5cfe9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:21 GMT  
		Size: 119.7 MB (119700912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
