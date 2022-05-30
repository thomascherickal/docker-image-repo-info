## `dart:stable`

```console
$ docker pull dart@sha256:2bfc343571aedaee7d0f15e753ef3eef1f666a66946e26ed7739c0c734cd88da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:e9eec5a88f4edc5d290427a200f212a3e70d6bc6010d2916519983c3aa6e44d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275806124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0579ebfe8fb79df236b037224d41fb1164e8d2ec1aeb1cf78ed03362563c8890`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:59:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:59:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:59:42 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:59:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:59:42 GMT
WORKDIR /root
# Sat, 28 May 2022 02:59:54 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=57b8fd964e47c81d467aeb95b099a670ab7e8f54a1cd74d45bcd1fdc77913d86;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c522ca1744de506276d19c1a5c120526daec142d2d7595d6915f77838066c2e8;             SDK_ARCH="arm";;         arm64)             DART_SHA256=05a1db0fd84585877d6180858346d7c53c7ef89433667db3b85f3f2e5fa7036b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cce345d47500dcf4216b5a3c3573997d8cee6ced941226cdad49cf3a05d9e4f`  
		Last Modified: Sat, 28 May 2022 03:00:25 GMT  
		Size: 45.1 MB (45073288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e7a1a5c2fc2560335de6071d4e7daaf8bfeb47ceba9ea5f63f45379314fe03`  
		Last Modified: Sat, 28 May 2022 03:00:18 GMT  
		Size: 2.1 MB (2139544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffee0224e60bcabd43c949268cefbe59ec8cd19dc59a5e920b5aae80e8f212da`  
		Last Modified: Sat, 28 May 2022 03:00:46 GMT  
		Size: 197.2 MB (197214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:7c6e8f157c8ddc5f12582597cbc4eb12e62a74b28b2aea469f691349bc7828ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184066674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fce6de09114ee63cff71c22d767aae913c899664b497cde5bfd66b7c871ff4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:22:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:22:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 03:22:23 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 03:22:23 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:22:24 GMT
WORKDIR /root
# Mon, 30 May 2022 17:57:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=696862ad8b7ecdceed43b85d4eb8279bc0f8dbb5b61b9e9afc86c54ecd7b40a2;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c2b3b3b8f5a5e21702ee59389ded2de4812d3239fd81a5ba82fd7f0442b7f2b7;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e796c032598392526ef2438c9cb5a4d146ffccadb0b9af1215eed322a39926a3;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c6d428b4fe22093e319eaeec2897112d388caefbdde84e76dca636416f42c`  
		Last Modified: Sat, 28 May 2022 03:24:22 GMT  
		Size: 41.0 MB (40966484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab852355c3b5ba6e8e4f2dc400200a47d5960f0584050eedaa94c7f98e8711e1`  
		Last Modified: Sat, 28 May 2022 03:23:58 GMT  
		Size: 1.3 MB (1288080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cee63f072adde413ace7363fe7d5b3b45266c5d6b16dd86ece41be69d05df3`  
		Last Modified: Mon, 30 May 2022 18:01:03 GMT  
		Size: 115.2 MB (115235873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:da59f635626bb8ba7c2694d3e80630cf9759e2a89b6811aca3414dfff52c1237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193155065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540b30075e2bb63e57a3be13f3c24d912e955b95d44cae613165e58ddb6404b3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:13:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:13:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 28 May 2022 02:13:47 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 28 May 2022 02:13:48 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:13:49 GMT
WORKDIR /root
# Mon, 30 May 2022 17:39:46 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=696862ad8b7ecdceed43b85d4eb8279bc0f8dbb5b61b9e9afc86c54ecd7b40a2;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c2b3b3b8f5a5e21702ee59389ded2de4812d3239fd81a5ba82fd7f0442b7f2b7;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e796c032598392526ef2438c9cb5a4d146ffccadb0b9af1215eed322a39926a3;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56dc0fade48cd32ac3c2827a832f3d61e45910be6637355d98dd1e0403f5ad9`  
		Last Modified: Sat, 28 May 2022 02:14:41 GMT  
		Size: 44.8 MB (44787670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a08645c0c3aebadcb4dfcda350fbd7c6476f3bffd877234348677ee6dc679e8`  
		Last Modified: Sat, 28 May 2022 02:14:35 GMT  
		Size: 1.6 MB (1556715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a1b077f7d15d9f92f176a730e59790ae2e60199c49b2bf257fcd3cbd43e387`  
		Last Modified: Mon, 30 May 2022 17:40:54 GMT  
		Size: 116.7 MB (116744952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
