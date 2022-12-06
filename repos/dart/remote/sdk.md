## `dart:sdk`

```console
$ docker pull dart@sha256:f2c0eea699e0366e5614e13761d12a9e193fb2ae8161aeed1999946e9e50c475
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:9a6a450b52fabc7c2a9e73fef3cf40de35d6ea1b029b69ff8c192b6efa568025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271971747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da9917698d10ec1cb862f0381ce7d962e5a428b51bfd2b8208ff5409a175c7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:25:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:25:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 06 Dec 2022 02:25:23 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 06 Dec 2022 02:25:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:25:24 GMT
WORKDIR /root
# Tue, 06 Dec 2022 02:25:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f64fbc5b90c6817d6f3a25cf9cec4277343cf265df233600838050639c593889;             SDK_ARCH="x64";;         armhf)             DART_SHA256=505df0bfcdb1a22b6486718f6833514926f39f4b28f390b3b67ef8fc7b149255;             SDK_ARCH="arm";;         arm64)             DART_SHA256=f8c6d7e1b0f090c536a64a6a130b065533efd83c290f4510f42325389a0c27a5;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a34df0b3a447c281ea06d9c3e6fd18f26e3005f46600a6c80991d5e097c441`  
		Last Modified: Tue, 06 Dec 2022 02:26:26 GMT  
		Size: 45.1 MB (45074515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e5662a2d3a834429c6d91698e1dc3cc23a6c8366f59c13112620b503c323d`  
		Last Modified: Tue, 06 Dec 2022 02:26:19 GMT  
		Size: 2.2 MB (2162024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a516c98f36a9d5e591d3e7c50bd43cd730111b712519ddd5b082e99d48624472`  
		Last Modified: Tue, 06 Dec 2022 02:26:46 GMT  
		Size: 193.3 MB (193322356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:e71ca639c9ae07cc35ee065f7d4db7835ee1a2f7471d97b82ddf7860ddf4d7f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180605712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a932a9c2fcad0bc3171033006b8c414f8b0c9a94e99627310045ae901a39a18`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:33:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:33:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 15 Nov 2022 12:33:12 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 15 Nov 2022 12:33:12 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 12:33:12 GMT
WORKDIR /root
# Fri, 25 Nov 2022 20:57:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f64fbc5b90c6817d6f3a25cf9cec4277343cf265df233600838050639c593889;             SDK_ARCH="x64";;         armhf)             DART_SHA256=505df0bfcdb1a22b6486718f6833514926f39f4b28f390b3b67ef8fc7b149255;             SDK_ARCH="arm";;         arm64)             DART_SHA256=f8c6d7e1b0f090c536a64a6a130b065533efd83c290f4510f42325389a0c27a5;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a060836b3eca611673ccd9d680e368afe1b43c4cca5c29daf2bf9ff5b11458`  
		Last Modified: Tue, 15 Nov 2022 12:34:41 GMT  
		Size: 41.0 MB (40956512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e54b8a06fcdc482f156780c911fc2d95e08e631c0b957a399dcc73e6628671`  
		Last Modified: Tue, 15 Nov 2022 12:34:34 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f7fa21b25d8bd7197a035bd6c8bd34c728b8ffc01670c579888c07eb3cf413`  
		Last Modified: Fri, 25 Nov 2022 20:59:11 GMT  
		Size: 111.8 MB (111784490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:772ba1b93dd5af93384267ce2c04156a91f350954d601949068f5a6a61f2eddd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189558844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a67e7fabe3bd23faab1461e746f3934e16e1d09afe5886ee320daadc6fa3a6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:39:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:39:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 06 Dec 2022 02:39:07 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 06 Dec 2022 02:39:07 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:39:07 GMT
WORKDIR /root
# Tue, 06 Dec 2022 02:39:16 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f64fbc5b90c6817d6f3a25cf9cec4277343cf265df233600838050639c593889;             SDK_ARCH="x64";;         armhf)             DART_SHA256=505df0bfcdb1a22b6486718f6833514926f39f4b28f390b3b67ef8fc7b149255;             SDK_ARCH="arm";;         arm64)             DART_SHA256=f8c6d7e1b0f090c536a64a6a130b065533efd83c290f4510f42325389a0c27a5;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d917a7e957b7ab720ebce685c3185d778f3797ecab94c98ed8b10e1153a968`  
		Last Modified: Tue, 06 Dec 2022 02:39:57 GMT  
		Size: 45.0 MB (44996085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c0c48988505b5210ac33bb7ef0500bab1289dde272bd14d2ef96f89e6480f1`  
		Last Modified: Tue, 06 Dec 2022 02:39:51 GMT  
		Size: 1.6 MB (1562183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d68bf61ad9163af8ab4e3891644e6bfd3abafa13d357851cdaaf22aed047f49`  
		Last Modified: Tue, 06 Dec 2022 02:40:04 GMT  
		Size: 112.9 MB (112940256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
