<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.19`](#dart219)
-	[`dart:2.19-sdk`](#dart219-sdk)
-	[`dart:2.19.6`](#dart2196)
-	[`dart:2.19.6-sdk`](#dart2196-sdk)
-	[`dart:3.0.0-290.3.beta`](#dart300-2903beta)
-	[`dart:3.0.0-290.3.beta-sdk`](#dart300-2903beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19-sdk`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19-sdk` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.6`

**does not exist** (yet?)

## `dart:2.19.6-sdk`

**does not exist** (yet?)

## `dart:3.0.0-290.3.beta`

```console
$ docker pull dart@sha256:f0c2088414ed054b04d71a9a1b3020a283ce7d49f3d6dc392b42d7acce90618d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.0-290.3.beta` - linux; amd64

```console
$ docker pull dart@sha256:ad14351ab7a71165b082e68565d1828e33b2dd091e5bc77d45b65f3eadf4aba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.8 MB (290844499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454260b9728679f4409ae930a1e5011f006d59a3e4a202b649c21a288c033bba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f6fe6060ed1381fb9241c167221e449f5b955cac018789c9a08911bb4d5811`  
		Last Modified: Fri, 24 Mar 2023 02:06:06 GMT  
		Size: 212.2 MB (212168406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.0-290.3.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:32a593435ea890ef0915b5ce13f965698b4e0f88ff69ca2e73987dc74e228696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186589501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a86a2708a250c3a67f2ed1e87e488b6652889293a459a23514d57a057856b90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390868485e0f579fb66d7c11f952388fa40e9f3366a591cce0d5b4cf86126b5`  
		Last Modified: Thu, 23 Mar 2023 23:42:16 GMT  
		Size: 117.7 MB (117735257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.0-290.3.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d39fb81e4a26ad78f3ce939e53e71603e23abc8324fcb77071779a76179ed629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195515044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25cc17ef1465a665766b50ea7d30d8245e14f961eda2809dcaa6b18cf71368e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c7f8e9e4d4cace5a36e918a040544179f3ce8294c77c6ea511d1910ec1861`  
		Last Modified: Thu, 23 Mar 2023 22:06:57 GMT  
		Size: 118.9 MB (118878969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:3.0.0-290.3.beta-sdk`

```console
$ docker pull dart@sha256:f0c2088414ed054b04d71a9a1b3020a283ce7d49f3d6dc392b42d7acce90618d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3.0.0-290.3.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:ad14351ab7a71165b082e68565d1828e33b2dd091e5bc77d45b65f3eadf4aba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.8 MB (290844499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454260b9728679f4409ae930a1e5011f006d59a3e4a202b649c21a288c033bba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f6fe6060ed1381fb9241c167221e449f5b955cac018789c9a08911bb4d5811`  
		Last Modified: Fri, 24 Mar 2023 02:06:06 GMT  
		Size: 212.2 MB (212168406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.0-290.3.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:32a593435ea890ef0915b5ce13f965698b4e0f88ff69ca2e73987dc74e228696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186589501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a86a2708a250c3a67f2ed1e87e488b6652889293a459a23514d57a057856b90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390868485e0f579fb66d7c11f952388fa40e9f3366a591cce0d5b4cf86126b5`  
		Last Modified: Thu, 23 Mar 2023 23:42:16 GMT  
		Size: 117.7 MB (117735257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3.0.0-290.3.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d39fb81e4a26ad78f3ce939e53e71603e23abc8324fcb77071779a76179ed629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195515044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25cc17ef1465a665766b50ea7d30d8245e14f961eda2809dcaa6b18cf71368e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c7f8e9e4d4cace5a36e918a040544179f3ce8294c77c6ea511d1910ec1861`  
		Last Modified: Thu, 23 Mar 2023 22:06:57 GMT  
		Size: 118.9 MB (118878969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:f0c2088414ed054b04d71a9a1b3020a283ce7d49f3d6dc392b42d7acce90618d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:ad14351ab7a71165b082e68565d1828e33b2dd091e5bc77d45b65f3eadf4aba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.8 MB (290844499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454260b9728679f4409ae930a1e5011f006d59a3e4a202b649c21a288c033bba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f6fe6060ed1381fb9241c167221e449f5b955cac018789c9a08911bb4d5811`  
		Last Modified: Fri, 24 Mar 2023 02:06:06 GMT  
		Size: 212.2 MB (212168406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:32a593435ea890ef0915b5ce13f965698b4e0f88ff69ca2e73987dc74e228696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186589501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a86a2708a250c3a67f2ed1e87e488b6652889293a459a23514d57a057856b90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390868485e0f579fb66d7c11f952388fa40e9f3366a591cce0d5b4cf86126b5`  
		Last Modified: Thu, 23 Mar 2023 23:42:16 GMT  
		Size: 117.7 MB (117735257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d39fb81e4a26ad78f3ce939e53e71603e23abc8324fcb77071779a76179ed629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195515044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25cc17ef1465a665766b50ea7d30d8245e14f961eda2809dcaa6b18cf71368e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c7f8e9e4d4cace5a36e918a040544179f3ce8294c77c6ea511d1910ec1861`  
		Last Modified: Thu, 23 Mar 2023 22:06:57 GMT  
		Size: 118.9 MB (118878969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:f0c2088414ed054b04d71a9a1b3020a283ce7d49f3d6dc392b42d7acce90618d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:ad14351ab7a71165b082e68565d1828e33b2dd091e5bc77d45b65f3eadf4aba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.8 MB (290844499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454260b9728679f4409ae930a1e5011f006d59a3e4a202b649c21a288c033bba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f6fe6060ed1381fb9241c167221e449f5b955cac018789c9a08911bb4d5811`  
		Last Modified: Fri, 24 Mar 2023 02:06:06 GMT  
		Size: 212.2 MB (212168406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:32a593435ea890ef0915b5ce13f965698b4e0f88ff69ca2e73987dc74e228696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186589501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a86a2708a250c3a67f2ed1e87e488b6652889293a459a23514d57a057856b90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390868485e0f579fb66d7c11f952388fa40e9f3366a591cce0d5b4cf86126b5`  
		Last Modified: Thu, 23 Mar 2023 23:42:16 GMT  
		Size: 117.7 MB (117735257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:d39fb81e4a26ad78f3ce939e53e71603e23abc8324fcb77071779a76179ed629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195515044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25cc17ef1465a665766b50ea7d30d8245e14f961eda2809dcaa6b18cf71368e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=eaaeee6be87a140a08ae0b6cc76e23ff4e5cb0ef7bbfa8ffa08b90e26b826e6e;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7636eb23c9053bceebf326ae46c8e7be57c5c3cbaedabe2a5a0d6c8717dcc5e9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b8f3d1f6c65657296757455ac99fab5772dcdb333cc83d15d626717779f2224a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.0.0-290.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c7f8e9e4d4cace5a36e918a040544179f3ce8294c77c6ea511d1910ec1861`  
		Last Modified: Thu, 23 Mar 2023 22:06:57 GMT  
		Size: 118.9 MB (118878969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:8f77135107ae6ac0a83cd80ae02c1515806f23133ad5d3b09902a138c274621a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:94c65fef2b24cfcfe1e07de04c3588bf306fe6a4f15ed5e0a73743b306656928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300574268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bef7f22d0367e8d16e9981d8fa94eff719911c41a22732632659419171902e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Fri, 24 Mar 2023 02:04:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a30e427a9c4205b05aab237b062dd4212b95cb84dddb97c0e4ee45da8aa5e`  
		Last Modified: Fri, 24 Mar 2023 02:05:17 GMT  
		Size: 221.9 MB (221898175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7b150904227cc2bf3690ae10eea862721c5a989f891a5e3a9b43c94a7511a769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8235fb07f90f51bc4f50cef44c2c1ab75f78ef21a212b685e39fe2f4945bfce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:21:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:06 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 13:21:06 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 13:21:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:21:06 GMT
WORKDIR /root
# Thu, 23 Mar 2023 23:40:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715e274c826ec94668b23f6888f73c60ffd0fa15aef470dcc46f9e15dc41ef6`  
		Last Modified: Thu, 23 Mar 2023 13:21:57 GMT  
		Size: 41.0 MB (40988373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ed017618896067a5d29e6a1ce57872dbc7c81a5a66dd647ed657fd0061279`  
		Last Modified: Thu, 23 Mar 2023 13:21:51 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c02cdc8f97be59d26e3bb3dac2cd531d9406d618ea60da783d29322ed7359`  
		Last Modified: Thu, 23 Mar 2023 23:41:36 GMT  
		Size: 127.9 MB (127903244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:34d31534de35f343bfb673b72cb30624dcb6f0066ab97c51f8bb7f3bc01fd3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6198b330e548892f5342a65fabc3c370c97cb5405b8d53108c933bf29b46000`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:23:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 07:23:51 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 07:23:51 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:23:51 GMT
WORKDIR /root
# Thu, 23 Mar 2023 22:05:41 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1c56de9877367f2ba9bd78f1916c8991a464301814e052e413186ea3f5edcaa5;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5f6773acaa41fda33cb266b0ad1968bc6d6fd2f876b43cab62692ac5273b0861;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e885c4a96fc578d3dd5db7bcb7d5d4f86a2cc3eebeacd12153787982e0f0ce10;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.5/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84eee815730fa9d95520548db8dafbf9297eada12fb2145488d3cd61c44ed9`  
		Last Modified: Thu, 23 Mar 2023 07:24:35 GMT  
		Size: 45.0 MB (45011196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c600577d34a9e7b16bf08f28f7dfdfe9f55eb6c443d6babd1b2b7ccda77fb655`  
		Last Modified: Thu, 23 Mar 2023 07:24:30 GMT  
		Size: 1.6 MB (1562179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c640d87d3f0e0d1d887b5ad0a05b5e79152d44a3ca4e10990406109c54792a`  
		Last Modified: Thu, 23 Mar 2023 22:06:23 GMT  
		Size: 129.4 MB (129351985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
