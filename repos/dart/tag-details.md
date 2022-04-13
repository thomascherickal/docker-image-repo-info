<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.16`](#dart216)
-	[`dart:2.16-sdk`](#dart216-sdk)
-	[`dart:2.16.2`](#dart2162)
-	[`dart:2.16.2-sdk`](#dart2162-sdk)
-	[`dart:2.17.0-266.1.beta`](#dart2170-2661beta)
-	[`dart:2.17.0-266.1.beta-sdk`](#dart2170-2661beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16-sdk`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16-sdk` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.2`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.2` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.2-sdk`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.0-266.1.beta`

**does not exist** (yet?)

## `dart:2.17.0-266.1.beta-sdk`

**does not exist** (yet?)

## `dart:beta`

```console
$ docker pull dart@sha256:86e373cbef7575ecf7abf4d416bc0f00b3b88855c44e0b267c41ee9c832e4691
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:c31a100325227f6b5788b546b1b8b9f77c442dbcf3fcfdd73a402248abe5f632
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278284433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991dd12434b8253705542aa7e297ce3766cf56e7f61d9661d680eadf866d4915`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Thu, 31 Mar 2022 04:45:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36af274e6315c77048d8944d3f0cd0cd38d4a08a69b35e21b5f252e2100c0e71`  
		Last Modified: Thu, 31 Mar 2022 04:45:59 GMT  
		Size: 199.7 MB (199693553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:f223e95a0a59196edfbdeab6f108a5908309e82a48b1c78039e63e3cab7c4397
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186845682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91cb93b2b09c16129202ee7d9d78d37dc650f6d604317ea6fa8ffb034f3da33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ae82c6d2779a292d9330c8faa02c04f1896d2ba364bb98a47941be03a7f915`  
		Last Modified: Wed, 30 Mar 2022 21:55:19 GMT  
		Size: 118.0 MB (118015553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0bd22c49e087375a177f7d1c0abee1024dfe21939e2be93c9c953f8e3e325c5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195927991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc1819217ca3ac6dbaacabf1a07f713e28036cc0eebbe80d5049252cd5669fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Thu, 31 Mar 2022 08:10:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6fe9ecdb641e2a22fe24a755aaeea464e2141f2d79d9c8247a741296d283c`  
		Last Modified: Thu, 31 Mar 2022 08:11:24 GMT  
		Size: 119.5 MB (119517508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:86e373cbef7575ecf7abf4d416bc0f00b3b88855c44e0b267c41ee9c832e4691
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:c31a100325227f6b5788b546b1b8b9f77c442dbcf3fcfdd73a402248abe5f632
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278284433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991dd12434b8253705542aa7e297ce3766cf56e7f61d9661d680eadf866d4915`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Thu, 31 Mar 2022 04:45:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36af274e6315c77048d8944d3f0cd0cd38d4a08a69b35e21b5f252e2100c0e71`  
		Last Modified: Thu, 31 Mar 2022 04:45:59 GMT  
		Size: 199.7 MB (199693553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:f223e95a0a59196edfbdeab6f108a5908309e82a48b1c78039e63e3cab7c4397
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186845682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91cb93b2b09c16129202ee7d9d78d37dc650f6d604317ea6fa8ffb034f3da33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ae82c6d2779a292d9330c8faa02c04f1896d2ba364bb98a47941be03a7f915`  
		Last Modified: Wed, 30 Mar 2022 21:55:19 GMT  
		Size: 118.0 MB (118015553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0bd22c49e087375a177f7d1c0abee1024dfe21939e2be93c9c953f8e3e325c5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195927991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc1819217ca3ac6dbaacabf1a07f713e28036cc0eebbe80d5049252cd5669fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Thu, 31 Mar 2022 08:10:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c2754bfd46b080c58699ba704ae8212c04ea8e907bec1d9d83d8768adfa587bc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a0575c89e7ceaf1a196929da07951dbc8d5333b2dbde49d456769f55aaaa70ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3834827f270d9c1fe285815339991ab7ee5862a6b3c647af933a8206a62a867f;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6fe9ecdb641e2a22fe24a755aaeea464e2141f2d79d9c8247a741296d283c`  
		Last Modified: Thu, 31 Mar 2022 08:11:24 GMT  
		Size: 119.5 MB (119517508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:05f96dee72162410837d919ec0250fa7e46ba38000b46505774cd3875001ecbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:1dd6a6feeee238e12deb8a9cfd7c45c93e545a9bddd0d77934b1f471ef955932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279616084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7474f655bc6f29714442db223d1b1223ca2945e52c30790870a6846b9ae2c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:45:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:45:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 29 Mar 2022 17:45:53 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 29 Mar 2022 17:45:53 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 17:45:54 GMT
WORKDIR /root
# Tue, 29 Mar 2022 17:46:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f2555ee8e1d058a6a21c44149f22779e3a9c548f9fead125028706e1ee699`  
		Last Modified: Tue, 29 Mar 2022 17:46:51 GMT  
		Size: 45.1 MB (45072878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bdf86bbdd984efc950a42c237605d8bc9d6e8cde4b21c8b7297123a345f3e`  
		Last Modified: Tue, 29 Mar 2022 17:46:44 GMT  
		Size: 2.1 MB (2139545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d5a4f8b43f486707d459ae4090339405982a5c681dae2e60ec91144730e2`  
		Last Modified: Tue, 29 Mar 2022 17:47:13 GMT  
		Size: 201.0 MB (201025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b972de46eb24f117322cfa6ecedfa998a90be7a96b66d0e81ad9f4794f947009
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187019668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cddc6f08ecff845daa06369c1595ccdf6e6421c1673ead0f583af9a6fe83a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 21:49:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 21:49:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 21:49:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 21:49:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 21:49:43 GMT
WORKDIR /root
# Wed, 30 Mar 2022 21:50:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82dffa22f8daa2ba79755d9d7468a2c3a642da5654d231a2a2bf3406ace9914`  
		Last Modified: Wed, 30 Mar 2022 21:52:25 GMT  
		Size: 41.0 MB (40966675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d8112f6894d4be8f01a13f51bdba197a6f75bba4b585b34ff314a26a21526`  
		Last Modified: Wed, 30 Mar 2022 21:52:01 GMT  
		Size: 1.3 MB (1288084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c7ebe5ce5fdee07791a2c6adb320c27c1a21df35b92dc81f89d43a840a166`  
		Last Modified: Wed, 30 Mar 2022 21:53:17 GMT  
		Size: 118.2 MB (118189539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f0cf607ff8213f126f10f795bcb0594e2ed5f0fcfe4086c8ccbaa6fb03c542e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196111380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97e2313b29928a177edca6e950ff6ba179618d2b38022730baced772ad768a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:33:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 30 Mar 2022 02:33:17 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 30 Mar 2022 02:33:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 02:33:19 GMT
WORKDIR /root
# Wed, 30 Mar 2022 02:33:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7a0ad877b0785e19018873c8144db3a29c4ab50e7c1aa968800280fd47a25e72;             SDK_ARCH="x64";;         armhf)             DART_SHA256=6eb58d7721bb27827d2bbb0830f3479c0e1d4c257b1c4c802ab8811c7938b02f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=be67ab8d79140149c8f058cafbadaa2ea8044e603e04b3c4657171c18a48f8a6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a423e5736d56d1e654dc7ea718c973984c74081bc9b6ea10355a237c6b0be05`  
		Last Modified: Wed, 30 Mar 2022 02:34:28 GMT  
		Size: 44.8 MB (44789449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2b4a6eab11a627b70631d84ed29f1de4e160d27ed55ae8e732e0c1ff17b1ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:22 GMT  
		Size: 1.6 MB (1556723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8355e18c2ca0af58af1daeca149fc5d71117ccf1ba87a9e48e4b25b3c35006`  
		Last Modified: Wed, 30 Mar 2022 02:34:39 GMT  
		Size: 119.7 MB (119700897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
