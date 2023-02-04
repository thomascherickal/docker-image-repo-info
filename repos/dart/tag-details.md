<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.19`](#dart219)
-	[`dart:2.19-sdk`](#dart219-sdk)
-	[`dart:2.19.1`](#dart2191)
-	[`dart:2.19.1-sdk`](#dart2191-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19-sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.1`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.1` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.1` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.1` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.1-sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.1-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.1-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.1-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:86d317e7e92835424db0263cd0cef52c7317aac51925846ead49178b7108189a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e3dd1b39a4dc1eaa18c2b4b22ea83aa6311f78188792c78b303a0b43e4c0e3ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514d6efa7042462655cb0b900dfc40137d65364f47255278d65f3cc2d78e2a3e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:33:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:33:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 07:33:07 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 07:33:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 07:33:07 GMT
WORKDIR /root
# Sat, 04 Feb 2023 07:33:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1ceb43b500f385991126667444cf67d9c43323882139a739b33b51d6d35afc`  
		Last Modified: Sat, 04 Feb 2023 07:33:49 GMT  
		Size: 45.1 MB (45101534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b5a4e90381f0050fb095acf5124e2fb9cb98210b17221e9eddbe4a3f176a16`  
		Last Modified: Sat, 04 Feb 2023 07:33:42 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a4d640d96df89aecfd3d5bba723416c681ddb70318aa8079ad029c7a9c16ae`  
		Last Modified: Sat, 04 Feb 2023 07:34:14 GMT  
		Size: 221.9 MB (221898670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:4a69bc072ec583e776036edeb9ff7bfdd71a150382ab7827511a83ec98da1c00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196707729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b08e82ebf589fb5faff03d62c9ae9b836115042652fb92693b8ee847d054a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:05:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:05:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 11:05:58 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 11:05:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 11:05:58 GMT
WORKDIR /root
# Sat, 04 Feb 2023 11:06:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6c5816589b4549ba41221fda6b67454b10685933602c15faab13a6ef9af42`  
		Last Modified: Sat, 04 Feb 2023 11:06:56 GMT  
		Size: 41.0 MB (40987505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c99b74f405a114ab4bc5c9901a0c83af93116ed7b449e471a16d50823b101`  
		Last Modified: Sat, 04 Feb 2023 11:06:49 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591b11c44eb3d9f85d1c2f84ad64712c1666e50862af5fc2f9e926b5dd3e125`  
		Last Modified: Sat, 04 Feb 2023 11:07:14 GMT  
		Size: 127.9 MB (127872237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:3c9996f8ec75117d15046b610d2b93b84f17909c53af89e395965984200a96e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205945949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a1110a7b169f68bbb6f84764a7742fc03f863fdaa244d74eb2ac5e01ebeed6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:56:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:56:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 04 Feb 2023 06:56:43 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 04 Feb 2023 06:56:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 06:56:43 GMT
WORKDIR /root
# Sat, 04 Feb 2023 06:56:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1390ab623dab8e6c23036e865cc8b6245476797f69c4c855e41bf9ff45928263;             SDK_ARCH="x64";;         armhf)             DART_SHA256=80b8abc7b3425561712bad6f6d7123217a26fa7697f8aac6dbf0e1e89ee6ea53;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ba6ccdf8d73ada5be6533cf58a97044ef1180e2d0cd4c7e17da21b62bca65042;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2c857f9031f1928346d5a7013fef3c248a5ee290ea78540b9ef451786cf9`  
		Last Modified: Sat, 04 Feb 2023 06:57:18 GMT  
		Size: 45.0 MB (45009357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57c837d524850bdc639ce14b14dfc733d64899b719ca687282f76b3db7d6241`  
		Last Modified: Sat, 04 Feb 2023 06:57:13 GMT  
		Size: 1.6 MB (1562173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65212c00c6e09623e7f0d937583e3cf5ed9f6b3de7f9883e109302b23f99c962`  
		Last Modified: Sat, 04 Feb 2023 06:57:28 GMT  
		Size: 129.3 MB (129329627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
