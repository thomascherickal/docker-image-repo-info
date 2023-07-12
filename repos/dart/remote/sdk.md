## `dart:sdk`

```console
$ docker pull dart@sha256:0334fa2254fe50fb9ddab78a362e12f5db8876e48bc25221347bf9d5bbb61c33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:d1650d51bed355c3ece66d1e8aca6cfbe863ba9ed2ce88bda61b5fbde1fc3704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296636072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0204a37fb0489934d6831c9cf4de22420aea16f22cb03695182ec9286769c`
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
# Wed, 12 Jul 2023 19:19:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:28558d2d719bf9776f60f047a0a4776240e677501155205d678a1e40abe2b4a6`  
		Last Modified: Wed, 12 Jul 2023 19:20:47 GMT  
		Size: 218.0 MB (217956390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9efeba686374829962d163dab883d7e7c6b4377888ebe77bceb45790094de983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191284603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eca39523f19cad218571ff97ff8d546180025f359a243ed529f5442d0747f5`
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
# Wed, 12 Jul 2023 18:57:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:d263f707f946aec095cfe3f437704252a027b0c7451ac333c204d2ffe338d983`  
		Last Modified: Wed, 12 Jul 2023 18:58:24 GMT  
		Size: 122.4 MB (122429775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7445905b856621801c7ad68f10365e3e4ae1975567155ed994e5fdc9855954f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200470410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab65e3daa1c5366083bcdc2951db610c99148d3e4d0baacdb175e9f1c0baceb`
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
# Wed, 12 Jul 2023 20:14:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=22138e69f9880514971f3de366902ddac89a5b9c2a593295f18fa1ec2f79e1c1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=10c6242e8a11b81424b6e5e0417c1c7be8eaabead585c2b113055b3236ff7434;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3ee243327167bf4675581ae4748df3c822b8600324b17ac5ed0b6cd14ec2981b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:50e90bc7c164e40366d18458a19cf49c8611a3e6e1ebe82a4df2b02ae07a6e79`  
		Last Modified: Wed, 12 Jul 2023 20:15:09 GMT  
		Size: 123.8 MB (123834662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
