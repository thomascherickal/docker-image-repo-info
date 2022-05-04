## `dart:beta`

```console
$ docker pull dart@sha256:f1a56a5162deb215a8640fe5cd071c805a0ee3e49bfb9ef37ff347a8f53f3cf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:63ff60883736b48f179d795bbe555054a131ed0bc9b3e67185cd860bc3bf1e4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275782376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efef526ddfc1e4ad2a0fe3402680bdd4812a0f33f871bd7a4ae89f4f93a5c929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 27 Apr 2022 20:43:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=c1417589e4ab70d79a88fafdd417bea30919c6026858f930cd5b7c976752afb6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=48faf51274672c4953ede2659c409f1bcf788e867421008df160956a6e03817f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=0bc1d229ecf27f084cc091feccfcd819a9281434362f45363632cfa8cb44c68a;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.7.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146e45ad8037b6f4f4b6b685d0807336bec2dbb6cd45402357048e6a93ffa33a`  
		Last Modified: Wed, 27 Apr 2022 20:44:50 GMT  
		Size: 197.2 MB (197191152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:80b970435f1bd03c887fb1a1f4394131460a350d27dd13742b9e992657ab5f99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184074728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26395769c60583745ac64ce304a2c5e685ba26ee394fcb09cfc89c3308c10c7a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 04 May 2022 17:58:18 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1cc4f69696674baace0a7f1b99668633f9fca51cfa1fbe716cc97f8289e59508;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e86ecd5f14c4a0de28569d3367e68600f1400c4a9a22792bc926a4368bebdb6a;             SDK_ARCH="arm";;         arm64)             DART_SHA256=18f98494af1e6d41fb0481ee010aee54b3ebfd72cad313ec2e067c1bb37e1968;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c55eb0afc08ec5e40099bc3d7d7d0b18e90d69a67f0dd717b6ef2f3c08e7c`  
		Last Modified: Wed, 04 May 2022 18:01:00 GMT  
		Size: 115.2 MB (115244218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f265132eba6ac7a665b67a41596ffae5e6339aae02bcee11e6ac9e595aa0658c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193152075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d93635a5ccb96e1a0f5940da361da8512b735fe1946760b576786a60fe0ffd4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 04 May 2022 17:39:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1cc4f69696674baace0a7f1b99668633f9fca51cfa1fbe716cc97f8289e59508;             SDK_ARCH="x64";;         armhf)             DART_SHA256=e86ecd5f14c4a0de28569d3367e68600f1400c4a9a22792bc926a4368bebdb6a;             SDK_ARCH="arm";;         arm64)             DART_SHA256=18f98494af1e6d41fb0481ee010aee54b3ebfd72cad313ec2e067c1bb37e1968;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.8.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3fdf05651da8cc75e00f564cd7bc2aa69e5697f0c251665bae970588ce1974`  
		Last Modified: Wed, 04 May 2022 17:40:50 GMT  
		Size: 116.7 MB (116740397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
