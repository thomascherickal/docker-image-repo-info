<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:3`](#dart3)
-	[`dart:3-sdk`](#dart3-sdk)
-	[`dart:3.0`](#dart30)
-	[`dart:3.0-sdk`](#dart30-sdk)
-	[`dart:3.0.4`](#dart304)
-	[`dart:3.0.4-sdk`](#dart304-sdk)
-	[`dart:3.1.0-163.1.beta`](#dart310-1631beta)
-	[`dart:3.1.0-163.1.beta-sdk`](#dart310-1631beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:3`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3-sdk`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0-sdk`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0-sdk` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.4`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.4` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.4` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.4` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.4-sdk`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.4-sdk` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.4-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.4-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-163.1.beta`

```console
$ docker pull dart@sha256:733006b90a05551af1fa6465afa23d074346f658eeb316bfb3cce6fb0d1df6d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1.0-163.1.beta` - linux; amd64

```console
$ docker pull dart@sha256:e987a41aae1b7f5ea6667118208c9549087c0d028d9209c5a528000e8051f724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286753987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5536218121a2a670077d1116caaafbfdbb011ae6e3c29b4c13b7e87b3d3f08`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:54:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11a9fc3b7634c5450c15b0eefc87d1320c26447a95e3846eae56f3c87926a7`  
		Last Modified: Tue, 13 Jun 2023 05:55:51 GMT  
		Size: 208.1 MB (208073175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-163.1.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5c3d6e51f1d0a8ac3eaae3e2fbbe9d30d700f2cf48ea30173b022b9856ec9def
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178824063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adccddc7723746563c5866b60e880fbdd67fa38f428788fdcc11a6b108a982`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1f7c729c3fd002a0e78a933e8ad62aaddab4ad5f68c02e6b014123505825d`  
		Last Modified: Thu, 08 Jun 2023 16:58:56 GMT  
		Size: 110.0 MB (109983365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-163.1.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f7cd4aa6a158304d6967436c0da05657098ff42b0990a4ddbb3fc47724a73b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187986888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c185c862462a854b1b115e512428873b02cb5ca7184426a571adf52e02726a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036117dbabdbdd829e1fc19eeeb32595f45984c0f9867fb037f5efb42b3d1967`  
		Last Modified: Tue, 13 Jun 2023 05:31:22 GMT  
		Size: 111.4 MB (111351945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.1.0-163.1.beta-sdk`

```console
$ docker pull dart@sha256:733006b90a05551af1fa6465afa23d074346f658eeb316bfb3cce6fb0d1df6d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.1.0-163.1.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e987a41aae1b7f5ea6667118208c9549087c0d028d9209c5a528000e8051f724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286753987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5536218121a2a670077d1116caaafbfdbb011ae6e3c29b4c13b7e87b3d3f08`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:54:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11a9fc3b7634c5450c15b0eefc87d1320c26447a95e3846eae56f3c87926a7`  
		Last Modified: Tue, 13 Jun 2023 05:55:51 GMT  
		Size: 208.1 MB (208073175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-163.1.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5c3d6e51f1d0a8ac3eaae3e2fbbe9d30d700f2cf48ea30173b022b9856ec9def
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178824063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adccddc7723746563c5866b60e880fbdd67fa38f428788fdcc11a6b108a982`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1f7c729c3fd002a0e78a933e8ad62aaddab4ad5f68c02e6b014123505825d`  
		Last Modified: Thu, 08 Jun 2023 16:58:56 GMT  
		Size: 110.0 MB (109983365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.1.0-163.1.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f7cd4aa6a158304d6967436c0da05657098ff42b0990a4ddbb3fc47724a73b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187986888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c185c862462a854b1b115e512428873b02cb5ca7184426a571adf52e02726a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036117dbabdbdd829e1fc19eeeb32595f45984c0f9867fb037f5efb42b3d1967`  
		Last Modified: Tue, 13 Jun 2023 05:31:22 GMT  
		Size: 111.4 MB (111351945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:733006b90a05551af1fa6465afa23d074346f658eeb316bfb3cce6fb0d1df6d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:e987a41aae1b7f5ea6667118208c9549087c0d028d9209c5a528000e8051f724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286753987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5536218121a2a670077d1116caaafbfdbb011ae6e3c29b4c13b7e87b3d3f08`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:54:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11a9fc3b7634c5450c15b0eefc87d1320c26447a95e3846eae56f3c87926a7`  
		Last Modified: Tue, 13 Jun 2023 05:55:51 GMT  
		Size: 208.1 MB (208073175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5c3d6e51f1d0a8ac3eaae3e2fbbe9d30d700f2cf48ea30173b022b9856ec9def
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178824063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adccddc7723746563c5866b60e880fbdd67fa38f428788fdcc11a6b108a982`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1f7c729c3fd002a0e78a933e8ad62aaddab4ad5f68c02e6b014123505825d`  
		Last Modified: Thu, 08 Jun 2023 16:58:56 GMT  
		Size: 110.0 MB (109983365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f7cd4aa6a158304d6967436c0da05657098ff42b0990a4ddbb3fc47724a73b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187986888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c185c862462a854b1b115e512428873b02cb5ca7184426a571adf52e02726a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036117dbabdbdd829e1fc19eeeb32595f45984c0f9867fb037f5efb42b3d1967`  
		Last Modified: Tue, 13 Jun 2023 05:31:22 GMT  
		Size: 111.4 MB (111351945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:733006b90a05551af1fa6465afa23d074346f658eeb316bfb3cce6fb0d1df6d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:e987a41aae1b7f5ea6667118208c9549087c0d028d9209c5a528000e8051f724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286753987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5536218121a2a670077d1116caaafbfdbb011ae6e3c29b4c13b7e87b3d3f08`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:54:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11a9fc3b7634c5450c15b0eefc87d1320c26447a95e3846eae56f3c87926a7`  
		Last Modified: Tue, 13 Jun 2023 05:55:51 GMT  
		Size: 208.1 MB (208073175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5c3d6e51f1d0a8ac3eaae3e2fbbe9d30d700f2cf48ea30173b022b9856ec9def
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178824063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adccddc7723746563c5866b60e880fbdd67fa38f428788fdcc11a6b108a982`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1f7c729c3fd002a0e78a933e8ad62aaddab4ad5f68c02e6b014123505825d`  
		Last Modified: Thu, 08 Jun 2023 16:58:56 GMT  
		Size: 110.0 MB (109983365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f7cd4aa6a158304d6967436c0da05657098ff42b0990a4ddbb3fc47724a73b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187986888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c185c862462a854b1b115e512428873b02cb5ca7184426a571adf52e02726a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036117dbabdbdd829e1fc19eeeb32595f45984c0f9867fb037f5efb42b3d1967`  
		Last Modified: Tue, 13 Jun 2023 05:31:22 GMT  
		Size: 111.4 MB (111351945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:63521c58feced290ecfa1500ebc868558583d260870404bb46fbc1490b228960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:59f20a0f74baf1bf908608134f16dd1c5ed8ae91d0194c05a925d3966c36a335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a1d84f868287029331a530a56b594660258ddebe526d750165e12bd4fc92d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:53:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c6350085c718b88d4e2e005023d4905cf882f1cac939f6c08140920ac98ae`  
		Last Modified: Tue, 13 Jun 2023 05:55:04 GMT  
		Size: 218.0 MB (217954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:65c1f406556dc8e62ca40f6b4a645b38fa8652d3876125b0b032d954528ebd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191270713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b100ade1ae68396d31a86e9284c85bf48e70fee4c0b0bdb0db9ac735603a81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:32:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:32:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 May 2023 06:32:48 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 May 2023 06:32:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:32:48 GMT
WORKDIR /root
# Thu, 08 Jun 2023 16:57:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b6b0696f49f6e66ff6f0496b056ebd7e9633d23ad4b260343c03d61dbed6`  
		Last Modified: Tue, 23 May 2023 06:33:34 GMT  
		Size: 41.0 MB (40988340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c024fad8b517f23c3bed43fde74e4a7171250c6f3596db921d6d7cacb0c71792`  
		Last Modified: Tue, 23 May 2023 06:33:28 GMT  
		Size: 1.3 MB (1287723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af040f4619d2dee7b6da41dd4519cbd2cc9ba629e60b592de4c2da0f6533a724`  
		Last Modified: Thu, 08 Jun 2023 16:58:17 GMT  
		Size: 122.4 MB (122430015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:60cbdf783a0a374071c9ce1dee419fa972d9aa28a08e6560152946243431ad78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200466719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c84ac79afa83a0586669dd01a0256ee0bb40a7d08b1603fc55e3c1a9bd77f5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:09 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=fed758732d742df884d39770756eb9bd9fdb24665c24c96502a09e03a745fca5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=36aebf7bf6d43574dc3f66872e1926e184dd2ef8641212240e57ab895403a967;             SDK_ARCH="arm";;         arm64)             DART_SHA256=d04dee8e097cdfe02f7aa2d51620104ac680291f9d3b772a7c788694e0934fc1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.0.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee818e2587b5743fce22a8393dd333ff63a216f9a078b66556057f90f7f205`  
		Last Modified: Tue, 13 Jun 2023 05:30:49 GMT  
		Size: 123.8 MB (123831776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
