## `dart:2-sdk`

```console
$ docker pull dart@sha256:194953ed1daa471d0d7af2e93e7337d7d7fc0e3003e87d85f96b90b1e6b601ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:fe8f8aea9ab797115994769c6384b43dbb76ada9697f67c619b218ef75a87f6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271978916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24270561242d45513a90b98fb9bd2f7af54946df580a899f54f1e25c99c80e78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:57:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:57:10 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Sep 2022 03:57:10 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Sep 2022 03:57:10 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 03:57:10 GMT
WORKDIR /root
# Tue, 13 Sep 2022 03:57:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e391c4ed8f623b9748f897cb585d629057c1141f9eaf8e9b2be118932ba11632;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2e83b4a03a9210713a2c65d2c50bd680984c414c3c89d78baba5a20f378fac7d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=06dd7c6eb6c903f5df8b23f9a35f7b1c35ccb869be6b5019c7dd93868ae2bfbf;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d63b6474cd1858e80830a661cd94266316317015c29b48065f8ca8f4be032b2`  
		Last Modified: Tue, 13 Sep 2022 03:57:52 GMT  
		Size: 45.1 MB (45076266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3e6f150bf6765ed0be2d60b823b718ea7bd975a53d61d41868af1dc4ac11e`  
		Last Modified: Tue, 13 Sep 2022 03:57:45 GMT  
		Size: 2.2 MB (2161955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04ebf3b32d586f07e955b65b8239c351efb1ce321feb6a66ec8ab205f4e0fd9`  
		Last Modified: Tue, 13 Sep 2022 03:58:13 GMT  
		Size: 193.3 MB (193336574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:25cce3da2027dc3c73cd98970a33f907d41fbf5c300182bc81d2ff0280158864
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180574620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aafa7db6ae9a0e838939a71d517ef2118d7b32c59a6b2058b7fa583b5b7d60d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:26:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:26:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Sep 2022 07:26:14 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Sep 2022 07:26:14 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 07:26:14 GMT
WORKDIR /root
# Thu, 15 Sep 2022 17:57:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7369fcbfb3c96ed85511224580a8ce0e5ecfc8227af563d396ede2055cdf84e1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=697361b627356224903e9e4fe4e9e2600a462c56fce04f31efbcff6a44ee47b7;             SDK_ARCH="arm";;         arm64)             DART_SHA256=1c8d96c0b718873f9ae6d9aa7d866cddefdb86f8b1584cbdf589670d65b7c167;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b1ef7c0532bd5fe661ea9cbf8603025c7072df6966b5e2eea270252e6dfad`  
		Last Modified: Tue, 13 Sep 2022 07:27:20 GMT  
		Size: 41.0 MB (40963731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6838c05dc76bf1457f69908db62b75bff01a7ad0947fe5d967f458d33a5ef07b`  
		Last Modified: Tue, 13 Sep 2022 07:27:10 GMT  
		Size: 1.3 MB (1288525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551f9f396189d88c319cdb390abadc2590d1ecf18fd87a34cfcd2a0ef8b3b38f`  
		Last Modified: Thu, 15 Sep 2022 17:59:41 GMT  
		Size: 111.8 MB (111755305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:46acc207a7f4005425e9aadb4a1830c7d084f9b8356e795e266c8e35d4db911a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189538767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa50b32d7155854b71ea47ff452d49bf3d3d4e21ccee89ffe6d7b98cfece8b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:14:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:14:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Sep 2022 05:14:16 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Sep 2022 05:14:17 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 05:14:18 GMT
WORKDIR /root
# Thu, 15 Sep 2022 17:46:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7369fcbfb3c96ed85511224580a8ce0e5ecfc8227af563d396ede2055cdf84e1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=697361b627356224903e9e4fe4e9e2600a462c56fce04f31efbcff6a44ee47b7;             SDK_ARCH="arm";;         arm64)             DART_SHA256=1c8d96c0b718873f9ae6d9aa7d866cddefdb86f8b1584cbdf589670d65b7c167;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a9bed1a37d8212c4127b7f476a6973c996f4cbd08e44efa25b860f6ad06ce`  
		Last Modified: Tue, 13 Sep 2022 05:15:09 GMT  
		Size: 45.0 MB (45003804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889d53a2fc31f3cb8044ed793a36d337b0f8a984b0edc1866293b36a9116b721`  
		Last Modified: Tue, 13 Sep 2022 05:15:03 GMT  
		Size: 1.6 MB (1556381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8d282a6b212dd41a844909c54759ba77f341f11c1630f4c3522d02a64e773`  
		Last Modified: Thu, 15 Sep 2022 17:48:00 GMT  
		Size: 112.9 MB (112924343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
