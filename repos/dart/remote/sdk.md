## `dart:sdk`

```console
$ docker pull dart@sha256:9e201c0ee32f0de9b30da39b121eac5089191c7144eecd33dc66cc0e088f8b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:516dac64be4274c9e71a3f7f9d201e14926062e16d016015b3539a29f30be402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275816576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6eec245219757c43c946996335f67ff120e430288b8520531111fb48c791b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:59:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 12 Jul 2022 02:59:02 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 12 Jul 2022 02:59:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 02:59:02 GMT
WORKDIR /root
# Wed, 13 Jul 2022 19:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f917959e81624996e9066796ed3b4d6e571cbc880050ada2576bb98642763bb`  
		Last Modified: Tue, 12 Jul 2022 03:00:00 GMT  
		Size: 45.1 MB (45073315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71203ed23ff0af6379c663fda23420d4da991909927621bc682b67d48328d642`  
		Last Modified: Tue, 12 Jul 2022 02:59:53 GMT  
		Size: 2.1 MB (2139541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db5f167beb94a382856673cdf9e4db6a8bc0ff33673640a9e7dd01d15e5836b`  
		Last Modified: Wed, 13 Jul 2022 19:20:34 GMT  
		Size: 197.2 MB (197237110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:dbef0b864ccd8c428016e97b686087bf18e936cb19c39da6981e2270868cb3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184073047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d639dc3aefeeb101d8e2b9e56f0573c15c3b3d14ead1dc45e1f684b8f0a01f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 14:07:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 14:07:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 28 Jul 2022 14:07:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 28 Jul 2022 14:07:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 14:07:39 GMT
WORKDIR /root
# Thu, 28 Jul 2022 14:08:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc5597d389fa3aa42fc7fe49ba96d5bcd9b38b37e5ed048e6cbab5fe03f084`  
		Last Modified: Thu, 28 Jul 2022 14:10:01 GMT  
		Size: 41.0 MB (40966367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a198e6c8834cc2647ec1af248db6233acda5dfd04ad69a32ff8f376f106a485`  
		Last Modified: Thu, 28 Jul 2022 14:09:39 GMT  
		Size: 1.3 MB (1288070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64aea2111e1e1c3bebc8949a8ffa3a6cec5250fb3df7f967c4d02f4558a32f`  
		Last Modified: Thu, 28 Jul 2022 14:10:27 GMT  
		Size: 115.3 MB (115258051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:65415d039d31a5ee2f0da4e411b585ced94dba98b374a68184b7062709727da5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193348235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03578b3cf4006076d204840b10c90b3a3b8428619e6cfe113c3cab780f01f234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:57:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:57:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 02 Aug 2022 01:57:17 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 02 Aug 2022 01:57:18 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 01:57:19 GMT
WORKDIR /root
# Tue, 02 Aug 2022 01:57:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca11465a33ff97f96ad800a64a57e83929ecd90e2c771dabb10d8b84f6b133fd`  
		Last Modified: Tue, 02 Aug 2022 01:58:28 GMT  
		Size: 45.0 MB (45002676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384c3bf9f217cd2a47032beadd3caf03b877ae2fe1dfaa8d7e3e5dc23bc20a1c`  
		Last Modified: Tue, 02 Aug 2022 01:58:22 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f5730efbdec63d5e44b4ed118854dc2daa64fbdb3fad26354fcb5edcd55a4e`  
		Last Modified: Tue, 02 Aug 2022 01:58:38 GMT  
		Size: 116.7 MB (116734534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
