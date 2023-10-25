<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:3`](#dart3)
-	[`dart:3-sdk`](#dart3-sdk)
-	[`dart:3.1`](#dart31)
-	[`dart:3.1-sdk`](#dart31-sdk)
-	[`dart:3.1.5`](#dart315)
-	[`dart:3.1.5-sdk`](#dart315-sdk)
-	[`dart:3.2.0-210.3.beta`](#dart320-2103beta)
-	[`dart:3.2.0-210.3.beta-sdk`](#dart320-2103beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:3`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3-sdk`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1-sdk`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1-sdk` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.5`

```console
$ docker pull dart@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `dart:3.1.5-sdk`

```console
$ docker pull dart@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `dart:3.2.0-210.3.beta`

```console
$ docker pull dart@sha256:b81805d66a633f8ee5bb20db229d7a680dd6ef16d1ef67fd74ca8a056f29a42f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.2.0-210.3.beta` - linux; amd64

```console
$ docker pull dart@sha256:a1fedf327725f42891ed4fb295c466842fc53dab725cff2babacf7e7f7ae24df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308566098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db7ed24a511c0754178ac14253b73098625411c109fd8691881eb8a4d9fc138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c987877cc19cbd0aa4001b940a525dff824ef8878bab87684783da58c8496ab5`  
		Last Modified: Thu, 19 Oct 2023 00:40:35 GMT  
		Size: 223.0 MB (222976393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.2.0-210.3.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5e89e24606972fea2d0a02a7d8ad161244ed6f1c1969931f81f57a7a6c31c22f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203524551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad825f4ce5572a3ed021ec4984ee3db92a6a867791a47638e331cd00fefda9f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242a5ac9e830f9d65b5eb965ec3a44637927b5718d0fe0b06499180ec2c23b0`  
		Last Modified: Thu, 19 Oct 2023 01:18:51 GMT  
		Size: 128.4 MB (128351037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.2.0-210.3.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c9ef4e296d2292b396fef7c1cd988672157ebc84864e2ac9e5f0564f7667189d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307154643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e56877ddb1201838c5e15bb54ca396a3432cf186f1775951ef8a8e13bf6ec8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:25:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cee90ac8206c9cc8c5dcab46dc5ed954fa47b0d2b3dec794ea21d22d95e62d`  
		Last Modified: Thu, 19 Oct 2023 01:26:57 GMT  
		Size: 222.2 MB (222162935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.2.0-210.3.beta-sdk`

```console
$ docker pull dart@sha256:b81805d66a633f8ee5bb20db229d7a680dd6ef16d1ef67fd74ca8a056f29a42f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.2.0-210.3.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a1fedf327725f42891ed4fb295c466842fc53dab725cff2babacf7e7f7ae24df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308566098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db7ed24a511c0754178ac14253b73098625411c109fd8691881eb8a4d9fc138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c987877cc19cbd0aa4001b940a525dff824ef8878bab87684783da58c8496ab5`  
		Last Modified: Thu, 19 Oct 2023 00:40:35 GMT  
		Size: 223.0 MB (222976393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.2.0-210.3.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5e89e24606972fea2d0a02a7d8ad161244ed6f1c1969931f81f57a7a6c31c22f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203524551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad825f4ce5572a3ed021ec4984ee3db92a6a867791a47638e331cd00fefda9f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242a5ac9e830f9d65b5eb965ec3a44637927b5718d0fe0b06499180ec2c23b0`  
		Last Modified: Thu, 19 Oct 2023 01:18:51 GMT  
		Size: 128.4 MB (128351037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.2.0-210.3.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c9ef4e296d2292b396fef7c1cd988672157ebc84864e2ac9e5f0564f7667189d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307154643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e56877ddb1201838c5e15bb54ca396a3432cf186f1775951ef8a8e13bf6ec8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:25:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cee90ac8206c9cc8c5dcab46dc5ed954fa47b0d2b3dec794ea21d22d95e62d`  
		Last Modified: Thu, 19 Oct 2023 01:26:57 GMT  
		Size: 222.2 MB (222162935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:b81805d66a633f8ee5bb20db229d7a680dd6ef16d1ef67fd74ca8a056f29a42f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:a1fedf327725f42891ed4fb295c466842fc53dab725cff2babacf7e7f7ae24df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308566098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db7ed24a511c0754178ac14253b73098625411c109fd8691881eb8a4d9fc138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c987877cc19cbd0aa4001b940a525dff824ef8878bab87684783da58c8496ab5`  
		Last Modified: Thu, 19 Oct 2023 00:40:35 GMT  
		Size: 223.0 MB (222976393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5e89e24606972fea2d0a02a7d8ad161244ed6f1c1969931f81f57a7a6c31c22f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203524551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad825f4ce5572a3ed021ec4984ee3db92a6a867791a47638e331cd00fefda9f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242a5ac9e830f9d65b5eb965ec3a44637927b5718d0fe0b06499180ec2c23b0`  
		Last Modified: Thu, 19 Oct 2023 01:18:51 GMT  
		Size: 128.4 MB (128351037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c9ef4e296d2292b396fef7c1cd988672157ebc84864e2ac9e5f0564f7667189d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307154643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e56877ddb1201838c5e15bb54ca396a3432cf186f1775951ef8a8e13bf6ec8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:25:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cee90ac8206c9cc8c5dcab46dc5ed954fa47b0d2b3dec794ea21d22d95e62d`  
		Last Modified: Thu, 19 Oct 2023 01:26:57 GMT  
		Size: 222.2 MB (222162935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:b81805d66a633f8ee5bb20db229d7a680dd6ef16d1ef67fd74ca8a056f29a42f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a1fedf327725f42891ed4fb295c466842fc53dab725cff2babacf7e7f7ae24df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308566098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db7ed24a511c0754178ac14253b73098625411c109fd8691881eb8a4d9fc138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c987877cc19cbd0aa4001b940a525dff824ef8878bab87684783da58c8496ab5`  
		Last Modified: Thu, 19 Oct 2023 00:40:35 GMT  
		Size: 223.0 MB (222976393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5e89e24606972fea2d0a02a7d8ad161244ed6f1c1969931f81f57a7a6c31c22f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203524551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad825f4ce5572a3ed021ec4984ee3db92a6a867791a47638e331cd00fefda9f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:26 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242a5ac9e830f9d65b5eb965ec3a44637927b5718d0fe0b06499180ec2c23b0`  
		Last Modified: Thu, 19 Oct 2023 01:18:51 GMT  
		Size: 128.4 MB (128351037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c9ef4e296d2292b396fef7c1cd988672157ebc84864e2ac9e5f0564f7667189d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307154643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e56877ddb1201838c5e15bb54ca396a3432cf186f1775951ef8a8e13bf6ec8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:25:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b3aa85b15bd13d619ba924524d5c7f082dc256a062ad34fe12ec824c9f05c2b3;             SDK_ARCH="x64";;         armhf)             DART_SHA256=08ec044e8b77a46d89073b5e312848b8f65b00f93a62aecd902613cef0ad1f9d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b7644435c8acf1e73da3f1ce16889b7222fbab37a75111aff225422a1cc61cab;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cee90ac8206c9cc8c5dcab46dc5ed954fa47b0d2b3dec794ea21d22d95e62d`  
		Last Modified: Thu, 19 Oct 2023 01:26:57 GMT  
		Size: 222.2 MB (222162935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:75e61c42ce2a0dbc9b4058e9ed4a94b32f056eada02af35cb32133a4ce783671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:2ca3a42fc6645beb9c97118e69ba70f5a706073fcd35f52092270d9b3ee3f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296151825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ec53d8a7c831969ec3364500dc5997c76aa567063007f454718f883b6b2c6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Thu, 19 Oct 2023 00:38:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa2d382f48202b84cb378903b9f4f6b5ea0099092fa2322c0b6391700310558`  
		Last Modified: Thu, 19 Oct 2023 00:39:40 GMT  
		Size: 210.6 MB (210562120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:37f4500e165237bd8a802c3baeb544bfec583f7bf014a0111f6859baee77183f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b25e88667d0103fd6f95330c26057c97705656699bf95498524031c8957531`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:17:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ab69c44d1d36819bb6764658a4a8aa217e98f90ec651ed0eb3968c0d55aa6`  
		Last Modified: Thu, 19 Oct 2023 01:18:07 GMT  
		Size: 111.9 MB (111926835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b62f9444832ffbd18a1f13ae0afcb0d793e55aa0b0204c358c4575c8ee5e86a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294668318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e016c8089b7b6e1ee1e1bb706be56a3b633710c40c9ac9b415b7b321a42b5dd6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 19 Oct 2023 01:24:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=280fcd1edba1b59af8a2d4b578904d25428ccff6e865c44bbfb5434d5cc02ddb;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d0ead2f833959fa4f33f8469fad933c3040774a050f3af58462e3c3840d258ef;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e65aa7084bd87f1d752b3070bb8c22fb85080fef12432db11eed8ed0cb0c99c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a4a340e119cb716628cc30f2466d72ae3861224c65be0631bc2891932e142`  
		Last Modified: Thu, 19 Oct 2023 01:26:06 GMT  
		Size: 209.7 MB (209676610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
