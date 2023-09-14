## `dart:3-sdk`

```console
$ docker pull dart@sha256:a57751bdedde962da08789236b12fd3793c10d43a473ef3e73c894d61740fb2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:3-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6d62d48ba8191a723c52a4cc26dc07267314bfaeefc9af4a923683e77a107a70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291211967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e550fe77da39e611d028497486d736a8c191f8b299beb6a52679fa1340053a1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:44:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:44:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 07 Sep 2023 03:44:20 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 07 Sep 2023 03:44:20 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:44:20 GMT
WORKDIR /root
# Wed, 13 Sep 2023 22:19:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=be679ccef3a0b28f19e296dd5b6374ac60dd0deb06d4d663da9905190489d48b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0be45ee5992be715cf57970f8b37f5be26d3be30202c420ce1606e10147223f0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=395180693ccc758e4e830d3b13c4879e6e96b6869763a56e91721bf9d4228250;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e157d41b26c9f503992d7e57319f59a2c5cab3165e562a6320ec4f3d181632`  
		Last Modified: Thu, 07 Sep 2023 03:45:21 GMT  
		Size: 45.1 MB (45101927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1ede03a6e9ae0fc777cd01694fa37bf19523f7881e4d107a8af209ffa72a0e`  
		Last Modified: Thu, 07 Sep 2023 03:45:15 GMT  
		Size: 2.2 MB (2160703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ecfd35de807c8104cc4bdf6e176704054956975a53088bf304adaccd320fa8`  
		Last Modified: Wed, 13 Sep 2023 22:20:30 GMT  
		Size: 212.5 MB (212531834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:2f86372e8e91d4dadc210b72bd08c7fc3f8cc9afe694df5b42a57a912943ca5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182227517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:717a055aee6de28bdaceb277a6b5efe5e06d2ceed9bcaa3e9e36f9b7e5a8de6a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:09 GMT
ADD file:d714939aacc810de397a02461ce4b9dd85e92783aff066bd3da685e3d2d97439 in / 
# Thu, 07 Sep 2023 00:58:10 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:55:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:55:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 07 Sep 2023 01:55:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 07 Sep 2023 01:55:59 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:55:59 GMT
WORKDIR /root
# Wed, 13 Sep 2023 21:57:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=be679ccef3a0b28f19e296dd5b6374ac60dd0deb06d4d663da9905190489d48b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0be45ee5992be715cf57970f8b37f5be26d3be30202c420ce1606e10147223f0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=395180693ccc758e4e830d3b13c4879e6e96b6869763a56e91721bf9d4228250;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:323242406c24248128abc25e113055d272350b4ac4ecd985dbabfb7061c48d49`  
		Last Modified: Thu, 07 Sep 2023 01:03:12 GMT  
		Size: 26.6 MB (26578710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aeaeabc9eed5e4b6207b4f729dc6c8f8acc154299578e082a7e1e6d570a18b6`  
		Last Modified: Thu, 07 Sep 2023 01:56:59 GMT  
		Size: 41.0 MB (40988287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7fe56ae6697aba2588a366d664e58dc3243c87d2f1ac39d7b64fe1a6a7914`  
		Last Modified: Thu, 07 Sep 2023 01:56:49 GMT  
		Size: 1.3 MB (1287721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a510e002775c32dd74af3337ec4f90c7460ed4caf0fc52dfcbc9d46ab2384a88`  
		Last Modified: Wed, 13 Sep 2023 21:58:04 GMT  
		Size: 113.4 MB (113372799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:3-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:7de2d7f4a577e26182636ec911fab99df60ccd31c1d2544cc9b3fd9acc656bcb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191389350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f44061be90e747a641e5da597e0cff30b358e6746909a83f8c7ba0cda123f1b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:22:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:22:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 07 Sep 2023 09:22:15 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 07 Sep 2023 09:22:15 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:22:15 GMT
WORKDIR /root
# Wed, 13 Sep 2023 22:39:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=be679ccef3a0b28f19e296dd5b6374ac60dd0deb06d4d663da9905190489d48b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0be45ee5992be715cf57970f8b37f5be26d3be30202c420ce1606e10147223f0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=395180693ccc758e4e830d3b13c4879e6e96b6869763a56e91721bf9d4228250;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788c40746a81524f09dd225e411210897fe94a5059d962757132e3ae53b6addf`  
		Last Modified: Thu, 07 Sep 2023 09:23:00 GMT  
		Size: 45.0 MB (45011532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8e74d1a76db5bc4404fba257d37be4abcd21feb13a407f79a8c12e64e6e924`  
		Last Modified: Thu, 07 Sep 2023 09:22:56 GMT  
		Size: 1.6 MB (1560882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03a1f12684ec03729ea07793e82da9086d9cbf24b3b2b46a9bca9b29a524f59`  
		Last Modified: Wed, 13 Sep 2023 22:39:58 GMT  
		Size: 114.8 MB (114754033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
