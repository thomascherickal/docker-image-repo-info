<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.16`](#dart216)
-	[`dart:2.16-sdk`](#dart216-sdk)
-	[`dart:2.16.1`](#dart2161)
-	[`dart:2.16.1-sdk`](#dart2161-sdk)
-	[`dart:2.17.0-69.2.beta`](#dart2170-692beta)
-	[`dart:2.17.0-69.2.beta-sdk`](#dart2170-692beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16-sdk`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.1`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.1` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.1` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.1` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.16.1-sdk`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.16.1-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.1-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.16.1-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.0-69.2.beta`

```console
$ docker pull dart@sha256:3fdd2f66ec4de962664bda69f3bd6ea3e1bcc883bc1172d8efa15a3973b60ffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.0-69.2.beta` - linux; amd64

```console
$ docker pull dart@sha256:6d3efc11d23a70bf2956ed7509ac92d9d5f0ba7996aae3faedcdc1934cbd640e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.4 MB (276437877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed4a0670df2a1792e24bd82ae91059bbc075963e20b240c7987f1244865a8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:20:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:20:54 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:20:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:20:54 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22a79674b3ee60d0932b66ebd872e46377f5de1e2f957b02e850222a37e61de`  
		Last Modified: Wed, 09 Feb 2022 20:21:38 GMT  
		Size: 45.1 MB (45071583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ca81ac51f5e17aadb887ac35143a0833ae40c25910b349f5598a0b44139246`  
		Last Modified: Wed, 09 Feb 2022 20:21:31 GMT  
		Size: 2.1 MB (2139226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e940d878a3abe9aad0f753aa52069bff8fbae64e733e4c511e77ff385f5166`  
		Last Modified: Tue, 15 Feb 2022 23:20:33 GMT  
		Size: 197.9 MB (197860811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-69.2.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:b648508f3aa8883ab9626ef2496cc54ffae0c03a36340366e3ed386e26b6fcd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185997606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c561160a3c46cf980ff8328a608c61ab01fe9048f92b67bbfa644e58b5a5dab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:58:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc258ef2e4e3ee5051c8cd0c6b48613770f29b4314ae3bc9fcb6d7e28bc7d35a`  
		Last Modified: Wed, 16 Feb 2022 00:01:32 GMT  
		Size: 117.2 MB (117184893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-69.2.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:409c5289dddf1201bc73ac2ce6908c83bc1ba456731190593625b7132f53c632
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195292047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa89655e74c901a23cdf92d120ec9295547fcca015ba494fcfc4889a4f0e8fe8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:40:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8263bd2d4143d0152642acbe62ac983844ee29aaa3e454ff5e8013d4002171cf`  
		Last Modified: Tue, 15 Feb 2022 23:41:03 GMT  
		Size: 118.7 MB (118686419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.17.0-69.2.beta-sdk`

```console
$ docker pull dart@sha256:47f358fa75207cb54958a6c9cdf52d63eadb2407931669995d09925b75b84045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.17.0-69.2.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:b6dc24d2c05f7d7cdf0fcef7623da367f80d969349a3bca84f1bcdaebe91a9a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.4 MB (276439933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:236574319f693fcea39779860b3703709e1fe3b29632860ced1649ca8b27081a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:24 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4b760d756a522da3e617513717044b6a609d151ac78e1092690ab7c617a7d3`  
		Last Modified: Tue, 01 Mar 2022 06:49:33 GMT  
		Size: 197.9 MB (197860746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-69.2.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b648508f3aa8883ab9626ef2496cc54ffae0c03a36340366e3ed386e26b6fcd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185997606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c561160a3c46cf980ff8328a608c61ab01fe9048f92b67bbfa644e58b5a5dab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:58:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc258ef2e4e3ee5051c8cd0c6b48613770f29b4314ae3bc9fcb6d7e28bc7d35a`  
		Last Modified: Wed, 16 Feb 2022 00:01:32 GMT  
		Size: 117.2 MB (117184893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.17.0-69.2.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:409c5289dddf1201bc73ac2ce6908c83bc1ba456731190593625b7132f53c632
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195292047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa89655e74c901a23cdf92d120ec9295547fcca015ba494fcfc4889a4f0e8fe8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:40:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8263bd2d4143d0152642acbe62ac983844ee29aaa3e454ff5e8013d4002171cf`  
		Last Modified: Tue, 15 Feb 2022 23:41:03 GMT  
		Size: 118.7 MB (118686419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:3fdd2f66ec4de962664bda69f3bd6ea3e1bcc883bc1172d8efa15a3973b60ffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:6d3efc11d23a70bf2956ed7509ac92d9d5f0ba7996aae3faedcdc1934cbd640e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.4 MB (276437877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed4a0670df2a1792e24bd82ae91059bbc075963e20b240c7987f1244865a8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:20:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:20:54 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:20:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:20:54 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22a79674b3ee60d0932b66ebd872e46377f5de1e2f957b02e850222a37e61de`  
		Last Modified: Wed, 09 Feb 2022 20:21:38 GMT  
		Size: 45.1 MB (45071583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ca81ac51f5e17aadb887ac35143a0833ae40c25910b349f5598a0b44139246`  
		Last Modified: Wed, 09 Feb 2022 20:21:31 GMT  
		Size: 2.1 MB (2139226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e940d878a3abe9aad0f753aa52069bff8fbae64e733e4c511e77ff385f5166`  
		Last Modified: Tue, 15 Feb 2022 23:20:33 GMT  
		Size: 197.9 MB (197860811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:b648508f3aa8883ab9626ef2496cc54ffae0c03a36340366e3ed386e26b6fcd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185997606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c561160a3c46cf980ff8328a608c61ab01fe9048f92b67bbfa644e58b5a5dab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:58:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc258ef2e4e3ee5051c8cd0c6b48613770f29b4314ae3bc9fcb6d7e28bc7d35a`  
		Last Modified: Wed, 16 Feb 2022 00:01:32 GMT  
		Size: 117.2 MB (117184893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:409c5289dddf1201bc73ac2ce6908c83bc1ba456731190593625b7132f53c632
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195292047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa89655e74c901a23cdf92d120ec9295547fcca015ba494fcfc4889a4f0e8fe8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:40:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8263bd2d4143d0152642acbe62ac983844ee29aaa3e454ff5e8013d4002171cf`  
		Last Modified: Tue, 15 Feb 2022 23:41:03 GMT  
		Size: 118.7 MB (118686419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:3fdd2f66ec4de962664bda69f3bd6ea3e1bcc883bc1172d8efa15a3973b60ffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6d3efc11d23a70bf2956ed7509ac92d9d5f0ba7996aae3faedcdc1934cbd640e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.4 MB (276437877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed4a0670df2a1792e24bd82ae91059bbc075963e20b240c7987f1244865a8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:20:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:20:54 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:20:54 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:20:54 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22a79674b3ee60d0932b66ebd872e46377f5de1e2f957b02e850222a37e61de`  
		Last Modified: Wed, 09 Feb 2022 20:21:38 GMT  
		Size: 45.1 MB (45071583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ca81ac51f5e17aadb887ac35143a0833ae40c25910b349f5598a0b44139246`  
		Last Modified: Wed, 09 Feb 2022 20:21:31 GMT  
		Size: 2.1 MB (2139226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e940d878a3abe9aad0f753aa52069bff8fbae64e733e4c511e77ff385f5166`  
		Last Modified: Tue, 15 Feb 2022 23:20:33 GMT  
		Size: 197.9 MB (197860811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b648508f3aa8883ab9626ef2496cc54ffae0c03a36340366e3ed386e26b6fcd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185997606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c561160a3c46cf980ff8328a608c61ab01fe9048f92b67bbfa644e58b5a5dab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:58:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc258ef2e4e3ee5051c8cd0c6b48613770f29b4314ae3bc9fcb6d7e28bc7d35a`  
		Last Modified: Wed, 16 Feb 2022 00:01:32 GMT  
		Size: 117.2 MB (117184893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:409c5289dddf1201bc73ac2ce6908c83bc1ba456731190593625b7132f53c632
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195292047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa89655e74c901a23cdf92d120ec9295547fcca015ba494fcfc4889a4f0e8fe8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Tue, 15 Feb 2022 23:40:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8263bd2d4143d0152642acbe62ac983844ee29aaa3e454ff5e8013d4002171cf`  
		Last Modified: Tue, 15 Feb 2022 23:41:03 GMT  
		Size: 118.7 MB (118686419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:58e34d0397051242528fa0ee1f843bd1ff4960b105401b0766903cfa3f82b990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:7c9216dd7d7941bdcca30a1e800b821894975a86e12c67c28a1e3b1989241d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279599415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2966378310e8018866671cdeee1149e820d022abf972eccd357a66c2572c9a25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:46:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:46:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 01 Mar 2022 06:46:46 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 01 Mar 2022 06:46:46 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 06:46:46 GMT
WORKDIR /root
# Tue, 01 Mar 2022 06:47:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed648f8ba452209b7d9a44ca13e17bebbea5f3e2560dd70a673c7e438b541f`  
		Last Modified: Tue, 01 Mar 2022 06:48:01 GMT  
		Size: 45.1 MB (45073567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb7dff545b6a6e052074de897e0687dc01cd764d96a04f1ebcaea3fde2e45d`  
		Last Modified: Tue, 01 Mar 2022 06:47:51 GMT  
		Size: 2.1 MB (2139224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b98a0af9ec88db1c6cfc7ae0f2abd20871aa1f0c667cc9ff13906f2e26d27d`  
		Last Modified: Tue, 01 Mar 2022 06:48:27 GMT  
		Size: 201.0 MB (201020228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7e9d225088706c233ef688a9c0ed4b01c2daf5fca0c8cb0e3ac561188e58fe27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (186998713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01ea6894cbd04aec70c07def0b1afc32d628edc8dd7152fb3d01edb0333e48c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 20:33:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 20:33:19 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 20:33:20 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 20:33:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 20:33:20 GMT
WORKDIR /root
# Wed, 09 Feb 2022 20:33:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43b50fceb916abe400cdb84c04833b6a1c1c8ede29daa0ecbf842fcfbc119e`  
		Last Modified: Wed, 09 Feb 2022 20:35:22 GMT  
		Size: 41.0 MB (40959881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afee36f184366b5058a73d2d8c2865eef7361970d26f20018be47185973d5bf6`  
		Last Modified: Wed, 09 Feb 2022 20:34:58 GMT  
		Size: 1.3 MB (1287899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f045dc12c66699698eb6dcdd778d75329e2322cbec959c019d8729d0224966`  
		Last Modified: Wed, 09 Feb 2022 20:36:14 GMT  
		Size: 118.2 MB (118186000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:4c450826677841ed8673cfd8d9ec1cf34c391b286efdcc606bba3432082251e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196305351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812e6a953d3fb52166a8f12bd9bf82a2a22baab7dce111113a07d92135e2abe5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 09 Feb 2022 21:03:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 09 Feb 2022 21:03:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 09 Feb 2022 21:03:48 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 09 Feb 2022 21:03:49 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Feb 2022 21:03:50 GMT
WORKDIR /root
# Wed, 09 Feb 2022 21:04:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3cc63a0c21500bc5eb9671733843dcc20040b39fdc02f35defcf7af59f88d459;             SDK_ARCH="x64";;         armhf)             DART_SHA256=16e0143716b3ad956fcec78bdb15834bcd67619e61ced0a7806328e9d385b2b3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=de9d1c528367f83bbd192bd565af5b7d9d48f76f79baa4c0e4cf64723e3fb8be;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.16.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2204074ce8e525c70293b1673017adc9a2f6fadaafeaa85e2904bfc1b7b7621`  
		Last Modified: Wed, 09 Feb 2022 21:04:40 GMT  
		Size: 45.0 MB (44992327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a53f8e60d58dac5940cafd832307395654e328d6ce05b4c16f42805f9bd3c3`  
		Last Modified: Wed, 09 Feb 2022 21:04:34 GMT  
		Size: 1.6 MB (1556527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02305769a3d972a6183d8108560ea55c8f45b3f8508c7a67ae6dbe1efac80b`  
		Last Modified: Wed, 09 Feb 2022 21:04:52 GMT  
		Size: 119.7 MB (119699723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
