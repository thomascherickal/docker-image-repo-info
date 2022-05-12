## `dart:beta-sdk`

```console
$ docker pull dart@sha256:ff9a0fde8b7961fd54089013b498cf5391b9ffd60a1e34a0bb69896e6d0e2ce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:b0f52dc3e2bdc8c43aec48a5651ee7839425b93445eeaa5c4a10638d848287fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275806106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb580b96172e96f493f79d929db3f71c77650812c43fb08796d531bd560823b3`
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
# Thu, 12 May 2022 04:38:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=57b8fd964e47c81d467aeb95b099a670ab7e8f54a1cd74d45bcd1fdc77913d86;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c522ca1744de506276d19c1a5c120526daec142d2d7595d6915f77838066c2e8;             SDK_ARCH="arm";;         arm64)             DART_SHA256=05a1db0fd84585877d6180858346d7c53c7ef89433667db3b85f3f2e5fa7036b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:d477575f8956a5b9813cc3211aca1fd7aa93c8f69de7cc0eb0438c253ea0c245`  
		Last Modified: Thu, 12 May 2022 04:38:51 GMT  
		Size: 197.2 MB (197214034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:054120c53a62bd7c0b019312ddc7475d95bcc22bc222d09064807fc214cc27c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ea740a32204548280ce11fbd8173136cf101082cd234a27c069fb5ead38b33`
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
# Wed, 11 May 2022 04:07:16 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1cc4f69696674baace0a7f1b99668633f9fca51cfa1fbe716cc97f8289e59508;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e86ecd5f14c4a0de28569d3367e68600f1400c4a9a22792bc926a4368bebdb6a;             SDK_ARCH="arm";;         arm64)             DART_SHA256=18f98494af1e6d41fb0481ee010aee54b3ebfd72cad313ec2e067c1bb37e1968;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:da0cb7ef13a312c1970c02d50610f6caf32ae3a0e0c593543f6788d1e0c8a1dc`  
		Last Modified: Wed, 11 May 2022 04:11:39 GMT  
		Size: 115.2 MB (115244282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4a2767d7986be2daea2eba31d266e80525cd64a52ddb5e238d367631835582a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5b9ddd5940125fb34ba28359aef0db4e990c2563ef36715c736caf32f250c7`
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
# Wed, 11 May 2022 14:12:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1cc4f69696674baace0a7f1b99668633f9fca51cfa1fbe716cc97f8289e59508;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e86ecd5f14c4a0de28569d3367e68600f1400c4a9a22792bc926a4368bebdb6a;             SDK_ARCH="arm";;         arm64)             DART_SHA256=18f98494af1e6d41fb0481ee010aee54b3ebfd72cad313ec2e067c1bb37e1968;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:0c5cb623fa6b3fe525abe9c051d50cb1c48bce55ecd7ae782fb75ea828bb11de`  
		Last Modified: Wed, 11 May 2022 14:14:19 GMT  
		Size: 116.7 MB (116740394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
