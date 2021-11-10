<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.14`](#dart214)
-	[`dart:2.14-sdk`](#dart214-sdk)
-	[`dart:2.14.4`](#dart2144)
-	[`dart:2.14.4-sdk`](#dart2144-sdk)
-	[`dart:2.15.0-268.8.beta`](#dart2150-2688beta)
-	[`dart:2.15.0-268.8.beta-sdk`](#dart2150-2688beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14-sdk`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14-sdk` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.4`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14.4` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.4-sdk`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.14.4-sdk` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.14.4-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-268.8.beta`

```console
$ docker pull dart@sha256:7768c3e2443c0867dc75a194f650adaeb979686607e2d7ea691b05aaf2759a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.15.0-268.8.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:0c74e5beeabd6d9c84486d6d5ba9d9819902de8eebeabde7be8d0d81c77790a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183679175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf35e2291d1ef0349bfc09b1e8315f9edfd6340fe97092af40b9c2f9b65a3e6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:01:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2b9971e04ac82b11b460e3571001d31d5d95c604d780a603bf172e8edc1bf`  
		Last Modified: Wed, 10 Nov 2021 20:03:57 GMT  
		Size: 115.2 MB (115185048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.15.0-268.8.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d99546980bffc38fd11ec3173a0c93519efc1e727670326585d195b32d8e1e3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193751883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6523303453badc92c571dd3ef9dc1b5bed5db8fbf254cc2175c8bb5c648565c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:08:34 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361e9fa74e5ccde8a6296f8585b4517cfbdfd292f1ba475ab535dbe2b881da9b`  
		Last Modified: Wed, 10 Nov 2021 20:09:31 GMT  
		Size: 116.6 MB (116572491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.15.0-268.8.beta-sdk`

```console
$ docker pull dart@sha256:7768c3e2443c0867dc75a194f650adaeb979686607e2d7ea691b05aaf2759a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.15.0-268.8.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:0c74e5beeabd6d9c84486d6d5ba9d9819902de8eebeabde7be8d0d81c77790a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183679175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf35e2291d1ef0349bfc09b1e8315f9edfd6340fe97092af40b9c2f9b65a3e6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:01:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2b9971e04ac82b11b460e3571001d31d5d95c604d780a603bf172e8edc1bf`  
		Last Modified: Wed, 10 Nov 2021 20:03:57 GMT  
		Size: 115.2 MB (115185048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.15.0-268.8.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d99546980bffc38fd11ec3173a0c93519efc1e727670326585d195b32d8e1e3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193751883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6523303453badc92c571dd3ef9dc1b5bed5db8fbf254cc2175c8bb5c648565c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:08:34 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361e9fa74e5ccde8a6296f8585b4517cfbdfd292f1ba475ab535dbe2b881da9b`  
		Last Modified: Wed, 10 Nov 2021 20:09:31 GMT  
		Size: 116.6 MB (116572491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:106d5b25ea8856784ce81432e306ff94e6769218762e4253afda2663bca868bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:8b61a918d91da3fdbf61df086b46cbc8f6f3d9ae2c112c4873120f52212bec14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283518150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7e4cbb3d8431173ba923d506886a861c90eb377b50586d3b8ca43fb59dc5c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0aa79c07ab059598b434fce574591ea5e318aefc579b3fe0b27e985fc5159270;             SDK_ARCH="x64";;         armhf)             DART_SHA256=4d0e0b9c0f30ecc2f65c4ff786948d99a06fa42a9191fe3be63efc56d40bafae;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e62e1ad98ada15b694641868c6d78c984796a12fcad74635db3527844130c875;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-178.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41596388168fa14583278ea9f7e2b576b950893118442ceb5c681a5752c7598f`  
		Last Modified: Wed, 20 Oct 2021 19:21:44 GMT  
		Size: 204.4 MB (204436910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:0c74e5beeabd6d9c84486d6d5ba9d9819902de8eebeabde7be8d0d81c77790a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183679175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf35e2291d1ef0349bfc09b1e8315f9edfd6340fe97092af40b9c2f9b65a3e6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:01:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2b9971e04ac82b11b460e3571001d31d5d95c604d780a603bf172e8edc1bf`  
		Last Modified: Wed, 10 Nov 2021 20:03:57 GMT  
		Size: 115.2 MB (115185048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d99546980bffc38fd11ec3173a0c93519efc1e727670326585d195b32d8e1e3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193751883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6523303453badc92c571dd3ef9dc1b5bed5db8fbf254cc2175c8bb5c648565c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:08:34 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361e9fa74e5ccde8a6296f8585b4517cfbdfd292f1ba475ab535dbe2b881da9b`  
		Last Modified: Wed, 10 Nov 2021 20:09:31 GMT  
		Size: 116.6 MB (116572491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:106d5b25ea8856784ce81432e306ff94e6769218762e4253afda2663bca868bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:8b61a918d91da3fdbf61df086b46cbc8f6f3d9ae2c112c4873120f52212bec14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283518150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7e4cbb3d8431173ba923d506886a861c90eb377b50586d3b8ca43fb59dc5c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0aa79c07ab059598b434fce574591ea5e318aefc579b3fe0b27e985fc5159270;             SDK_ARCH="x64";;         armhf)             DART_SHA256=4d0e0b9c0f30ecc2f65c4ff786948d99a06fa42a9191fe3be63efc56d40bafae;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e62e1ad98ada15b694641868c6d78c984796a12fcad74635db3527844130c875;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-178.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41596388168fa14583278ea9f7e2b576b950893118442ceb5c681a5752c7598f`  
		Last Modified: Wed, 20 Oct 2021 19:21:44 GMT  
		Size: 204.4 MB (204436910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:0c74e5beeabd6d9c84486d6d5ba9d9819902de8eebeabde7be8d0d81c77790a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.7 MB (183679175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf35e2291d1ef0349bfc09b1e8315f9edfd6340fe97092af40b9c2f9b65a3e6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:01:28 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2b9971e04ac82b11b460e3571001d31d5d95c604d780a603bf172e8edc1bf`  
		Last Modified: Wed, 10 Nov 2021 20:03:57 GMT  
		Size: 115.2 MB (115185048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d99546980bffc38fd11ec3173a0c93519efc1e727670326585d195b32d8e1e3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193751883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6523303453badc92c571dd3ef9dc1b5bed5db8fbf254cc2175c8bb5c648565c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 10 Nov 2021 20:08:34 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=91105c1ebc6bdf5c2b3f42cb8e22a51b80343d3a256117b6b1539a01232ecefc;             SDK_ARCH="x64";;         armhf)             DART_SHA256=60610240a6d1bab7389a71d84a40d6b40198d11784e4c49ee224ee611de1eebb;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c5396e6b36f38339cb36e34481e1e49de6de1f49fcecd82e370787d08659671e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.15.0-268.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361e9fa74e5ccde8a6296f8585b4517cfbdfd292f1ba475ab535dbe2b881da9b`  
		Last Modified: Wed, 10 Nov 2021 20:09:31 GMT  
		Size: 116.6 MB (116572491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:9757b5b8476e71d0be28730289214d681efb69900149a1eb4da7eccffac501b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:368597d56f8472ad1e46a036a3e4b42ce3d46b17a32a85aff9567d4dbc3ab98d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91437c5c4a3278fa297aef0ea82bc96c95aa1cd18aba10f2ffe3199eeb7d927c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:48:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 19:19:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 19:19:26 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 19:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 19:19:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 19:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0967f1c7a0cff360e1b4b316d95f992ede8dd65a5ce3d015aeabaad78b097d`  
		Last Modified: Tue, 12 Oct 2021 09:50:01 GMT  
		Size: 49.6 MB (49582550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64842add3dda57040a4df62a26e075094c4c400aac5366bdcacaf530d1220d4c`  
		Last Modified: Wed, 20 Oct 2021 19:20:19 GMT  
		Size: 2.4 MB (2359180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b162512271fc02eee130989346ee5601dd020f59496eefc2fdfff2b467ac7e`  
		Last Modified: Wed, 20 Oct 2021 19:20:47 GMT  
		Size: 210.0 MB (209985816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:737bb8c83ec5ac9ffd28a6d81ef72ab040e9d1e36298ecb7ad9ebe00d0f5fbed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190263050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8e0d8442d57586244bad25cbdcbd15ba28c2e90535a7d850023cb9c91974f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 20:55:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 20:56:01 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 20:56:02 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 20:56:02 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 20:56:03 GMT
WORKDIR /root
# Wed, 20 Oct 2021 20:56:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ca40230e9e81d005d24fbff784833e4b12d28f23ba19645a1a8881a7ebff89`  
		Last Modified: Wed, 20 Oct 2021 20:58:53 GMT  
		Size: 44.4 MB (44398524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f75fbf2d2dfa47b53fed470455e9230b58bd7efb0a9fc809c623df0853caf`  
		Last Modified: Wed, 20 Oct 2021 20:58:28 GMT  
		Size: 1.4 MB (1355905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6e805f8c0f57283976365fbe45d751d749c72a95cea1422d7130ab5f8c5e2e`  
		Last Modified: Wed, 20 Oct 2021 20:59:45 GMT  
		Size: 121.8 MB (121768923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:0db68003bc9fecfdf8c1b72cd5379e62a147f593afbd75aede8283ae4b757c45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200003807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afbbe833f791fb54076a8ac4d2b3e2b9d92abe9b493b0358e5b3d6ad0626b956`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 20 Oct 2021 18:44:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Oct 2021 18:44:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Oct 2021 18:44:24 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Oct 2021 18:44:25 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Oct 2021 18:44:26 GMT
WORKDIR /root
# Wed, 20 Oct 2021 18:44:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=49b6a98008ef546cb9c221461529d6c02cf2474bff098e0dc7e4ff1ef0f8a289;             SDK_ARCH="x64";;         armhf)             DART_SHA256=796b64022615ea75f05f20a3d5e7018e52a1d26c06acb1d2b0b2faa5df491a64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0477fae6fcff58fec18d912537f13d647fa0e137fce23401eea73102dce62351;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.14.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ddd8113ef38d17d67a4104cede247dccdae5d82c759bb8200adf5dd79777`  
		Last Modified: Wed, 20 Oct 2021 18:45:38 GMT  
		Size: 49.6 MB (49638983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dbc39b6a737a104b6c9a67ea9ed2c9e533d43dd1c9fb0d8d2eb1c5a3273e10`  
		Last Modified: Wed, 20 Oct 2021 18:45:32 GMT  
		Size: 1.6 MB (1631930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449b487b88a0a941881cd63be35e82182e2c49d8e7ed7de2e85a31894ba702`  
		Last Modified: Wed, 20 Oct 2021 18:45:48 GMT  
		Size: 122.8 MB (122824415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
