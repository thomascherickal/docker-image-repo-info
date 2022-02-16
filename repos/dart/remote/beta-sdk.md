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
