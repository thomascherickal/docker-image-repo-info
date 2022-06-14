<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.17`](#dart217)
-	[`dart:2.17-sdk`](#dart217-sdk)
-	[`dart:2.17.3`](#dart2173)
-	[`dart:2.17.3-sdk`](#dart2173-sdk)
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
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17-sdk`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.3`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.3` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.3` - linux; arm variant v7

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

### `dart:2.17.3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.3-sdk`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.3-sdk` - linux; arm variant v7

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

### `dart:2.17.3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-165.1.beta`

```console
$ docker pull dart@sha256:a3bda73453becc71def3543ee367709bca4322ddf108a61b24a9225fab1953b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:5ace16f585cf5ad434a603a8e9a6dd4937a907308fd16c6f5c059cd1e3971c8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a87d660eb4f46a45d8b21e41e0fbe5c275430b41d7b0882afde5a3d124f97b26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:19:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e8d9e332daee0e6a83352564357ae8522282f39cf805c3affbeb3e1c59a372`  
		Last Modified: Tue, 14 Jun 2022 18:20:35 GMT  
		Size: 202.0 MB (201992409 bytes)  
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
$ docker pull dart@sha256:4454bb4a14f187c6b7c0552b009afef82b4084aefcbdd30ee0f92434c67b2048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40c94c8f8dad8b2ba3e9bd7f5985a17b8e5e78dcb37f911d47c9f7dd79633f2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:39:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05115a827c9815f26546f7b3ec6e497ca7bf87944d0331bb131d48539506b9`  
		Last Modified: Tue, 14 Jun 2022 18:40:51 GMT  
		Size: 118.8 MB (118763171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.0-165.1.beta-sdk`

```console
$ docker pull dart@sha256:a3bda73453becc71def3543ee367709bca4322ddf108a61b24a9225fab1953b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.0-165.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:5ace16f585cf5ad434a603a8e9a6dd4937a907308fd16c6f5c059cd1e3971c8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a87d660eb4f46a45d8b21e41e0fbe5c275430b41d7b0882afde5a3d124f97b26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:19:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e8d9e332daee0e6a83352564357ae8522282f39cf805c3affbeb3e1c59a372`  
		Last Modified: Tue, 14 Jun 2022 18:20:35 GMT  
		Size: 202.0 MB (201992409 bytes)  
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
$ docker pull dart@sha256:4454bb4a14f187c6b7c0552b009afef82b4084aefcbdd30ee0f92434c67b2048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40c94c8f8dad8b2ba3e9bd7f5985a17b8e5e78dcb37f911d47c9f7dd79633f2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:39:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05115a827c9815f26546f7b3ec6e497ca7bf87944d0331bb131d48539506b9`  
		Last Modified: Tue, 14 Jun 2022 18:40:51 GMT  
		Size: 118.8 MB (118763171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:a3bda73453becc71def3543ee367709bca4322ddf108a61b24a9225fab1953b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:5ace16f585cf5ad434a603a8e9a6dd4937a907308fd16c6f5c059cd1e3971c8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a87d660eb4f46a45d8b21e41e0fbe5c275430b41d7b0882afde5a3d124f97b26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:19:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e8d9e332daee0e6a83352564357ae8522282f39cf805c3affbeb3e1c59a372`  
		Last Modified: Tue, 14 Jun 2022 18:20:35 GMT  
		Size: 202.0 MB (201992409 bytes)  
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
$ docker pull dart@sha256:4454bb4a14f187c6b7c0552b009afef82b4084aefcbdd30ee0f92434c67b2048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40c94c8f8dad8b2ba3e9bd7f5985a17b8e5e78dcb37f911d47c9f7dd79633f2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:39:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05115a827c9815f26546f7b3ec6e497ca7bf87944d0331bb131d48539506b9`  
		Last Modified: Tue, 14 Jun 2022 18:40:51 GMT  
		Size: 118.8 MB (118763171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:a3bda73453becc71def3543ee367709bca4322ddf108a61b24a9225fab1953b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:5ace16f585cf5ad434a603a8e9a6dd4937a907308fd16c6f5c059cd1e3971c8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.6 MB (280584517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a87d660eb4f46a45d8b21e41e0fbe5c275430b41d7b0882afde5a3d124f97b26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:19:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e8d9e332daee0e6a83352564357ae8522282f39cf805c3affbeb3e1c59a372`  
		Last Modified: Tue, 14 Jun 2022 18:20:35 GMT  
		Size: 202.0 MB (201992409 bytes)  
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
$ docker pull dart@sha256:4454bb4a14f187c6b7c0552b009afef82b4084aefcbdd30ee0f92434c67b2048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.2 MB (195173284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40c94c8f8dad8b2ba3e9bd7f5985a17b8e5e78dcb37f911d47c9f7dd79633f2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Tue, 14 Jun 2022 18:39:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=dc57e88d3c60cbd5ee738505fed804d854bfb1b30bdff9f218bb1d1085ec8173;             SDK_ARCH="x64";;         armhf)             DART_SHA256=34bd7665d677eb201c3eb78b8e26eb7d3ef05818815005869f0b166c59e1d909;             SDK_ARCH="arm";;         arm64)             DART_SHA256=99c787a521458e6fd3d402bff47f4b4c47c5ad32727f9b3a204310fc25e3b14a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.18.0-165.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05115a827c9815f26546f7b3ec6e497ca7bf87944d0331bb131d48539506b9`  
		Last Modified: Tue, 14 Jun 2022 18:40:51 GMT  
		Size: 118.8 MB (118763171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:3c3728c2979777d8b923fec7e91449242c4de4df9eda0659d9855448ade2a9bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d6079b2bed8af1a82af876ee8f98df30252cf8ddb13719747f4d21368b409622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275815918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46172e62aa52d287d2eda420523d25322b698847e11fa54ebcc00333c50950`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Wed, 01 Jun 2022 21:19:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2599514f65e54e6bb62e743687d4eadc0a623facfea5d02b400a4650daa1655f`  
		Last Modified: Wed, 01 Jun 2022 21:20:28 GMT  
		Size: 197.2 MB (197223810 bytes)  
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
$ docker pull dart@sha256:84b8c7343f319e5c98cf48258785d3b01fd39f24bdbc0eca808b7f65a6d64493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624080ab2354551982fdf75b3e319b1e0c612fbde93a2604ebb0d364b1a6c777`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Wed, 01 Jun 2022 20:39:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=68f9a09ac61aab1c135ad2e64a39bfac088900d439941dee275d8ea8c8541b95;             SDK_ARCH="x64";;         armhf)             DART_SHA256=75d1f5969ae12298d27b00bbe5866cdfcad422102929b52dc035c264ecc979a9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c993247b5adaab432fbb4d4b144d5a52c4c4011656312d2b008ef6ec51eaeadb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9d330553c0bb1a048ebaa5b8bb76c462ee8d83c78e8b4d1cf2ed493ddc240`  
		Last Modified: Wed, 01 Jun 2022 20:40:40 GMT  
		Size: 116.7 MB (116744900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
