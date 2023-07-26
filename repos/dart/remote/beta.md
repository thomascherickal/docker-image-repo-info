## `dart:beta`

```console
$ docker pull dart@sha256:71ea70ea0a59b4d5535a905885aa9402181f7ca51b18cfcc74101fbc164584d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:f93406dd56b7fdbe1189ad4f4c2cba6686c79a5553f6d5bbc3ac5dded6b58ad3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291213513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60ebc754b36e4b77f0feeaf597c18282c0cee3d31c70087eb350f623b694276`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:31:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:31:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 16:31:25 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 16:31:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:31:25 GMT
WORKDIR /root
# Wed, 26 Jul 2023 19:22:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e3bdf39358dda7f0fd02b25d4d4539536fff53b4ab257da31a5fbbe42edc28c9;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5a521eb74b6d65bfca7780c444b8e69f6d54bb541600bd94fedbec4b67200a3e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e7c2d1d4c8c8a6a47d916f422ddad2d5497307a147fa860b7b063ffdd162939;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a69116690feb3643215a073a6626dc504d416a560be4e49f95e558c3425424`  
		Last Modified: Tue, 04 Jul 2023 16:32:25 GMT  
		Size: 45.1 MB (45101591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf8f80bfd0002d5c55817d2feb51dff45eee12beaad28e8e5015fe1feca400`  
		Last Modified: Tue, 04 Jul 2023 16:32:19 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93e9f675f7b081ab21d74e6d1d788849b256d6f49d7ea2c548fdac26517e150`  
		Last Modified: Wed, 26 Jul 2023 19:24:23 GMT  
		Size: 212.5 MB (212533831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:6cce14f0f31761f84c1e7def39ab17f4c7a187fff105d23c688ffd9754607432
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182227512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f7a4c56465c46930988c141db1f593f932df8d9727f82b65d69ceaac8d8312`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:48:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 04:48:54 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 04:48:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 04:48:54 GMT
WORKDIR /root
# Wed, 26 Jul 2023 19:57:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e3bdf39358dda7f0fd02b25d4d4539536fff53b4ab257da31a5fbbe42edc28c9;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5a521eb74b6d65bfca7780c444b8e69f6d54bb541600bd94fedbec4b67200a3e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e7c2d1d4c8c8a6a47d916f422ddad2d5497307a147fa860b7b063ffdd162939;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1c528f6e0e6dc194afe817dfc0b005dd828845732b389e072ac0fde2cac59`  
		Last Modified: Tue, 04 Jul 2023 04:49:48 GMT  
		Size: 41.0 MB (40988364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc480ba96325e927880251a0fe41be000756e84091b4d4808c437d7145493e6`  
		Last Modified: Tue, 04 Jul 2023 04:49:42 GMT  
		Size: 1.3 MB (1287710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1cc7a4b9e21603e1e53e540ec5f78d0877ba094bda6dab43940b3a5dcea4ba`  
		Last Modified: Wed, 26 Jul 2023 19:59:00 GMT  
		Size: 113.4 MB (113372684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4bbb72b0fd84f66913fccc2864782f75b96861281c529b409258e48be9199785
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191391086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85884419b16b5b982a502ce88504696203430c2ba22c9b0d0d293972fe82004`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 04 Jul 2023 06:27:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 04 Jul 2023 06:27:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:50 GMT
WORKDIR /root
# Wed, 26 Jul 2023 19:41:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e3bdf39358dda7f0fd02b25d4d4539536fff53b4ab257da31a5fbbe42edc28c9;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5a521eb74b6d65bfca7780c444b8e69f6d54bb541600bd94fedbec4b67200a3e;             SDK_ARCH="arm";;         arm64)             DART_SHA256=7e7c2d1d4c8c8a6a47d916f422ddad2d5497307a147fa860b7b063ffdd162939;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-262.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858db84d271e12fd2a30055e0801bcad9e53fa0a8a44e4999b847efd6dbd615`  
		Last Modified: Tue, 04 Jul 2023 06:28:33 GMT  
		Size: 45.0 MB (45011923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3eec8396d4193294be339e2f7e47d0873c8513df2ad9780a7d728bcf74cace`  
		Last Modified: Tue, 04 Jul 2023 06:28:28 GMT  
		Size: 1.6 MB (1560868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eaaf22d82f1e167c40c8b3835320fbf181d8758f334b2d053ec5088c74ea91`  
		Last Modified: Wed, 26 Jul 2023 19:42:10 GMT  
		Size: 114.8 MB (114755338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
