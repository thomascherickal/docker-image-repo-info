<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.18`](#dart218)
-	[`dart:2.18-sdk`](#dart218-sdk)
-	[`dart:2.18.3`](#dart2183)
-	[`dart:2.18.3-sdk`](#dart2183-sdk)
-	[`dart:2.19.0-255.2.beta`](#dart2190-2552beta)
-	[`dart:2.19.0-255.2.beta-sdk`](#dart2190-2552beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18-sdk`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18-sdk` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.3`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.3` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.3` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.3-sdk`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18.3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18.3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.0-255.2.beta`

```console
$ docker pull dart@sha256:65138b3cbb561d2c9f7b2e6bf71454c10da097a61dc5e56d30a21bda22c34adc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.0-255.2.beta` - linux; amd64

```console
$ docker pull dart@sha256:7cb613446e88a5e38161e69bf99c6d3da18b32c3a12cebda3134af12cccf77ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274822875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e9866c60e4722c67bac462c6132e0b680abbcb263b27442b86885ce568f21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Thu, 06 Oct 2022 09:04:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c5cad7ed906d0d7c97cecc83e20327ad2c7c331332d9f0fe21785784424cb`  
		Last Modified: Thu, 06 Oct 2022 09:05:18 GMT  
		Size: 196.2 MB (196167306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:14afac02c33e4034c06a626c62fa43de7bab6b18ef78ecd1b0cb8b2e07d0cd59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca728506c7d80422bfde9000868ec3e375d77884978a40d08d66523f6a34a9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Thu, 06 Oct 2022 18:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fded9339682d613be49d1d0b16762221c34e97e8d75e245c968c107f66db75`  
		Last Modified: Thu, 06 Oct 2022 18:11:20 GMT  
		Size: 113.8 MB (113806159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c5bfc720f6b7ceb10efbf2c4623c630b7441b6c69d1ec443d131e83bed768272
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191403024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89d5dc9a6ae43eb4ea8bc98d91277b2eaa9ac6eaf6f33f9d5552a9a8d47ccb1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Thu, 06 Oct 2022 07:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070098b30b969901ce6bbb0808f19c71701e06eff0db07c51318d9ff69d2d99`  
		Last Modified: Thu, 06 Oct 2022 07:11:09 GMT  
		Size: 115.0 MB (114990499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.0-255.2.beta-sdk`

```console
$ docker pull dart@sha256:65138b3cbb561d2c9f7b2e6bf71454c10da097a61dc5e56d30a21bda22c34adc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.0-255.2.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7cb613446e88a5e38161e69bf99c6d3da18b32c3a12cebda3134af12cccf77ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274822875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e9866c60e4722c67bac462c6132e0b680abbcb263b27442b86885ce568f21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Thu, 06 Oct 2022 09:04:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c5cad7ed906d0d7c97cecc83e20327ad2c7c331332d9f0fe21785784424cb`  
		Last Modified: Thu, 06 Oct 2022 09:05:18 GMT  
		Size: 196.2 MB (196167306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:14afac02c33e4034c06a626c62fa43de7bab6b18ef78ecd1b0cb8b2e07d0cd59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca728506c7d80422bfde9000868ec3e375d77884978a40d08d66523f6a34a9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Thu, 06 Oct 2022 18:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fded9339682d613be49d1d0b16762221c34e97e8d75e245c968c107f66db75`  
		Last Modified: Thu, 06 Oct 2022 18:11:20 GMT  
		Size: 113.8 MB (113806159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c5bfc720f6b7ceb10efbf2c4623c630b7441b6c69d1ec443d131e83bed768272
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191403024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89d5dc9a6ae43eb4ea8bc98d91277b2eaa9ac6eaf6f33f9d5552a9a8d47ccb1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Thu, 06 Oct 2022 07:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070098b30b969901ce6bbb0808f19c71701e06eff0db07c51318d9ff69d2d99`  
		Last Modified: Thu, 06 Oct 2022 07:11:09 GMT  
		Size: 115.0 MB (114990499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:65138b3cbb561d2c9f7b2e6bf71454c10da097a61dc5e56d30a21bda22c34adc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:7cb613446e88a5e38161e69bf99c6d3da18b32c3a12cebda3134af12cccf77ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274822875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e9866c60e4722c67bac462c6132e0b680abbcb263b27442b86885ce568f21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Thu, 06 Oct 2022 09:04:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c5cad7ed906d0d7c97cecc83e20327ad2c7c331332d9f0fe21785784424cb`  
		Last Modified: Thu, 06 Oct 2022 09:05:18 GMT  
		Size: 196.2 MB (196167306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:14afac02c33e4034c06a626c62fa43de7bab6b18ef78ecd1b0cb8b2e07d0cd59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca728506c7d80422bfde9000868ec3e375d77884978a40d08d66523f6a34a9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Thu, 06 Oct 2022 18:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fded9339682d613be49d1d0b16762221c34e97e8d75e245c968c107f66db75`  
		Last Modified: Thu, 06 Oct 2022 18:11:20 GMT  
		Size: 113.8 MB (113806159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c5bfc720f6b7ceb10efbf2c4623c630b7441b6c69d1ec443d131e83bed768272
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191403024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89d5dc9a6ae43eb4ea8bc98d91277b2eaa9ac6eaf6f33f9d5552a9a8d47ccb1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Thu, 06 Oct 2022 07:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070098b30b969901ce6bbb0808f19c71701e06eff0db07c51318d9ff69d2d99`  
		Last Modified: Thu, 06 Oct 2022 07:11:09 GMT  
		Size: 115.0 MB (114990499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:65138b3cbb561d2c9f7b2e6bf71454c10da097a61dc5e56d30a21bda22c34adc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7cb613446e88a5e38161e69bf99c6d3da18b32c3a12cebda3134af12cccf77ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274822875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8e9866c60e4722c67bac462c6132e0b680abbcb263b27442b86885ce568f21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Thu, 06 Oct 2022 09:04:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c5cad7ed906d0d7c97cecc83e20327ad2c7c331332d9f0fe21785784424cb`  
		Last Modified: Thu, 06 Oct 2022 09:05:18 GMT  
		Size: 196.2 MB (196167306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:14afac02c33e4034c06a626c62fa43de7bab6b18ef78ecd1b0cb8b2e07d0cd59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca728506c7d80422bfde9000868ec3e375d77884978a40d08d66523f6a34a9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Thu, 06 Oct 2022 18:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fded9339682d613be49d1d0b16762221c34e97e8d75e245c968c107f66db75`  
		Last Modified: Thu, 06 Oct 2022 18:11:20 GMT  
		Size: 113.8 MB (113806159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:c5bfc720f6b7ceb10efbf2c4623c630b7441b6c69d1ec443d131e83bed768272
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191403024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89d5dc9a6ae43eb4ea8bc98d91277b2eaa9ac6eaf6f33f9d5552a9a8d47ccb1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Thu, 06 Oct 2022 07:10:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0070098b30b969901ce6bbb0808f19c71701e06eff0db07c51318d9ff69d2d99`  
		Last Modified: Thu, 06 Oct 2022 07:11:09 GMT  
		Size: 115.0 MB (114990499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:d879de36e41e411374970b3db0795f0f247d47cdd02c64d8dff2a7256d378f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:53504007b4816787cfdaf806e71a95ec71987cd4c1f5ff98e6e4ff16a6cc2228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271981201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92316bdf7cf308dd78156a0122ca84823b75e9c7f38999835f016b0043d92179`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:56:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:56:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:56:59 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:56:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:56:59 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:19:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4943a35aef482ebfb072b88347326a9068d39c832273f21e5bbe4420f5700f`  
		Last Modified: Wed, 05 Oct 2022 01:57:58 GMT  
		Size: 45.1 MB (45073499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e97eacefd681aa9637074b2f95ca3f7944d1ef18343dc170f00d4cd00580f`  
		Last Modified: Wed, 05 Oct 2022 01:57:51 GMT  
		Size: 2.2 MB (2161968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e85bbdb8b7d2004f80c263ab5b5623809f07888d8d16f1ccd8e3662eee3339d`  
		Last Modified: Wed, 19 Oct 2022 19:20:32 GMT  
		Size: 193.3 MB (193325632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:cf1c6a6d7fb3c481eb16a3dd61cc1c8d556f6e34f0b9f36573ca807055f21fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180602252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a8749f5d9c3fac4209c5d8a0962709b7e500b0def5829f129bb424c51931b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:07:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:07:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:07:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:07:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:07:03 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:57:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ba6dbb90fca59a02490ded2c70ae39d2370c99af2878d715cfe32456dc99`  
		Last Modified: Wed, 05 Oct 2022 01:08:34 GMT  
		Size: 41.0 MB (40956155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71f3a922ad3f4e673ec9d2b89cefc49bab9db492c408e780485e4d32f67de04`  
		Last Modified: Wed, 05 Oct 2022 01:08:22 GMT  
		Size: 1.3 MB (1288534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb97bd662b112ac0774fe6584d3c8bfba5889f267eaf6d93fcec5d9ca3219c`  
		Last Modified: Wed, 19 Oct 2022 19:59:04 GMT  
		Size: 111.8 MB (111778364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0d25c10402f7112521194a848ac3c59f1e15a4fc6c989da479f886e9475444bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189352174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed62df4eddf8501f7926039b2890d275f626ed31553b6e4c63ce9c5de01ccbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:22:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 05 Oct 2022 01:22:53 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 05 Oct 2022 01:22:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 01:22:55 GMT
WORKDIR /root
# Wed, 19 Oct 2022 19:39:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b1e9bf245b4ed8d0d5804b0b80ccf0d21d77250ae8bdaa46249bf97870964`  
		Last Modified: Wed, 05 Oct 2022 01:24:03 GMT  
		Size: 44.8 MB (44791748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266f3bb3cdeeb4fd1780909e2397c47d92bd68d7678de447c55f13da54b62ea`  
		Last Modified: Wed, 05 Oct 2022 01:23:56 GMT  
		Size: 1.6 MB (1556382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08d0c4441da78e8ab8eed9483a052b7e9193c90276159a2e94c54a1ce94aa78`  
		Last Modified: Wed, 19 Oct 2022 19:40:42 GMT  
		Size: 112.9 MB (112939649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
