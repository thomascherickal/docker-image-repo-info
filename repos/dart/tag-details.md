<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.17`](#dart217)
-	[`dart:2.17-sdk`](#dart217-sdk)
-	[`dart:2.17.5`](#dart2175)
-	[`dart:2.17.5-sdk`](#dart2175-sdk)
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
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17-sdk`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17-sdk` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.5`

```console
$ docker pull dart@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `dart:2.17.5-sdk`

```console
$ docker pull dart@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `dart:2.18.0-165.1.beta`

```console
$ docker pull dart@sha256:574d825bf9b62b9c745956cb6bf32a3e62f1eec9e75535a184b90ff545e4e1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:05fa6dd1df2263d4828e90fe2a821eb83054380c4ddaf8f98c38c0f0f6e0ee01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144175f6df2e16114318f9189436ac2dd4dfac8d4de60e15b2034278e73dd99d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6701c67576f75c6e1cbae400a63aaeff7b32ed114fd4bc0c54e150f3f8ddc9e`  
		Last Modified: Thu, 23 Jun 2022 01:11:45 GMT  
		Size: 202.0 MB (201992439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:2a66bcf26e4c4932fdb74fb3f6513692853139338a07f85c4e56f5fb1f99aeb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186076798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a5a666fb7a5c939314f041711fc67e894854ce242e47c16604162a28b20370`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Tue, 14 Jun 2022 17:58:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29348c84ccc03d85a66bc1025576a1bfd61469339834001b7debc7bac2a1fa2a`  
		Last Modified: Tue, 14 Jun 2022 18:01:03 GMT  
		Size: 117.2 MB (117245997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8b3f313cbefdcc3000d3bb50f9d9600c47b932051c83ee06c949649eca40fbbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0732728f32e035dd634c11e3010896cabcc8292c4df95a97fbe66b9661ce75d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:35:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3110ad2d95c63b0f0533534be8fd07e949e1f660d0115954f2f6f10164c6ba0`  
		Last Modified: Thu, 23 Jun 2022 01:36:43 GMT  
		Size: 118.8 MB (118763169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-165.1.beta-sdk`

```console
$ docker pull dart@sha256:574d825bf9b62b9c745956cb6bf32a3e62f1eec9e75535a184b90ff545e4e1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:05fa6dd1df2263d4828e90fe2a821eb83054380c4ddaf8f98c38c0f0f6e0ee01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144175f6df2e16114318f9189436ac2dd4dfac8d4de60e15b2034278e73dd99d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6701c67576f75c6e1cbae400a63aaeff7b32ed114fd4bc0c54e150f3f8ddc9e`  
		Last Modified: Thu, 23 Jun 2022 01:11:45 GMT  
		Size: 202.0 MB (201992439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:2a66bcf26e4c4932fdb74fb3f6513692853139338a07f85c4e56f5fb1f99aeb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186076798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a5a666fb7a5c939314f041711fc67e894854ce242e47c16604162a28b20370`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Tue, 14 Jun 2022 17:58:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29348c84ccc03d85a66bc1025576a1bfd61469339834001b7debc7bac2a1fa2a`  
		Last Modified: Tue, 14 Jun 2022 18:01:03 GMT  
		Size: 117.2 MB (117245997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.0-165.1.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8b3f313cbefdcc3000d3bb50f9d9600c47b932051c83ee06c949649eca40fbbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0732728f32e035dd634c11e3010896cabcc8292c4df95a97fbe66b9661ce75d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:35:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3110ad2d95c63b0f0533534be8fd07e949e1f660d0115954f2f6f10164c6ba0`  
		Last Modified: Thu, 23 Jun 2022 01:36:43 GMT  
		Size: 118.8 MB (118763169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:574d825bf9b62b9c745956cb6bf32a3e62f1eec9e75535a184b90ff545e4e1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:05fa6dd1df2263d4828e90fe2a821eb83054380c4ddaf8f98c38c0f0f6e0ee01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144175f6df2e16114318f9189436ac2dd4dfac8d4de60e15b2034278e73dd99d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6701c67576f75c6e1cbae400a63aaeff7b32ed114fd4bc0c54e150f3f8ddc9e`  
		Last Modified: Thu, 23 Jun 2022 01:11:45 GMT  
		Size: 202.0 MB (201992439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:2a66bcf26e4c4932fdb74fb3f6513692853139338a07f85c4e56f5fb1f99aeb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186076798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a5a666fb7a5c939314f041711fc67e894854ce242e47c16604162a28b20370`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Tue, 14 Jun 2022 17:58:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29348c84ccc03d85a66bc1025576a1bfd61469339834001b7debc7bac2a1fa2a`  
		Last Modified: Tue, 14 Jun 2022 18:01:03 GMT  
		Size: 117.2 MB (117245997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8b3f313cbefdcc3000d3bb50f9d9600c47b932051c83ee06c949649eca40fbbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0732728f32e035dd634c11e3010896cabcc8292c4df95a97fbe66b9661ce75d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:35:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3110ad2d95c63b0f0533534be8fd07e949e1f660d0115954f2f6f10164c6ba0`  
		Last Modified: Thu, 23 Jun 2022 01:36:43 GMT  
		Size: 118.8 MB (118763169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:574d825bf9b62b9c745956cb6bf32a3e62f1eec9e75535a184b90ff545e4e1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:05fa6dd1df2263d4828e90fe2a821eb83054380c4ddaf8f98c38c0f0f6e0ee01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144175f6df2e16114318f9189436ac2dd4dfac8d4de60e15b2034278e73dd99d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6701c67576f75c6e1cbae400a63aaeff7b32ed114fd4bc0c54e150f3f8ddc9e`  
		Last Modified: Thu, 23 Jun 2022 01:11:45 GMT  
		Size: 202.0 MB (201992439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:2a66bcf26e4c4932fdb74fb3f6513692853139338a07f85c4e56f5fb1f99aeb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186076798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a5a666fb7a5c939314f041711fc67e894854ce242e47c16604162a28b20370`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Tue, 14 Jun 2022 17:58:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29348c84ccc03d85a66bc1025576a1bfd61469339834001b7debc7bac2a1fa2a`  
		Last Modified: Tue, 14 Jun 2022 18:01:03 GMT  
		Size: 117.2 MB (117245997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8b3f313cbefdcc3000d3bb50f9d9600c47b932051c83ee06c949649eca40fbbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0732728f32e035dd634c11e3010896cabcc8292c4df95a97fbe66b9661ce75d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:35:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3110ad2d95c63b0f0533534be8fd07e949e1f660d0115954f2f6f10164c6ba0`  
		Last Modified: Thu, 23 Jun 2022 01:36:43 GMT  
		Size: 118.8 MB (118763169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:30168445d6b3dbee249e98b17ef7ce0882fd78f5308909e8f36dfdd5838852e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:06db9fcfb0d3c800747dd9d1db0b1c305b0310ea700b45841d43a0a2df205cf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d105d121cc50e0ce4c377de5270155a1568eb4609387e2a4827bd2804c46e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:09:23 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:09:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:09:23 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:09:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21038826bf36dd28993c0d8d4789901cbe65aafc668cc12dfbb576e4188ab354`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 45.1 MB (45073398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10969d89d09d31e83a8b64cadfb8d9c0de851813845b10e125795949d3af6e26`  
		Last Modified: Thu, 23 Jun 2022 01:10:19 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a097b144c274cd4eb99dc74068dd9b5c1b0ea8fcc2a0fb42faa4b7257a316d`  
		Last Modified: Thu, 23 Jun 2022 01:10:47 GMT  
		Size: 197.2 MB (197223778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:62d007a5b22a294cec951b307abf50cf4925088ceb2757536fa7a1e3828f5b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ba62a04386c2b0c7a456f34be34cd436d832ca4d003bae467f9bc5a8161373`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:57:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28e2ae3c4e7f466eb88bac0f4cca8b8ed576b23dc3f02ca6bcc1ccb62486bf7`  
		Last Modified: Wed, 01 Jun 2022 21:00:45 GMT  
		Size: 115.2 MB (115242330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:a574bc27666f021ffd38c48ec9353766888f8d30da68cd766a60a029b4247b43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193154859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e794eea398be2f05bccbe081e5ba9d3024d7c7440b41bd847b737c1fd9482cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:34:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:34:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Jun 2022 01:34:32 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Jun 2022 01:34:33 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 01:34:34 GMT
WORKDIR /root
# Thu, 23 Jun 2022 01:34:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a1846f0df3e092bed3ccbdb67b060ba83675fea74b289f2998817b451469d`  
		Last Modified: Thu, 23 Jun 2022 01:35:41 GMT  
		Size: 44.8 MB (44787526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac39ee64267cb16a3631042405e478e1baa5aac6bf458219b78ccca9f43d188`  
		Last Modified: Thu, 23 Jun 2022 01:35:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce364080633f795fa22d82c6ffbb5d3b3a2e8bada5bda743e869fb21d45b77`  
		Last Modified: Thu, 23 Jun 2022 01:35:51 GMT  
		Size: 116.7 MB (116744898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
