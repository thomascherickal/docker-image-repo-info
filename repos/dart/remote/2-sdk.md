## `dart:2-sdk`

```console
$ docker pull dart@sha256:f6ceb27c2b6d172020931d81a4f2721b341d718fdfd8fda508588d89c7bfae9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:a7000973c30c8554d569ccf164d6dc1381c1de81dfb481aaa26ae0e1455f2437
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271938375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25e7c10c0ae1890d05642d009207936af13b2ad228d5028ae7f233e6a120253`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 05:19:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 05:19:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 16 Nov 2022 05:19:13 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 16 Nov 2022 05:19:13 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 05:19:13 GMT
WORKDIR /root
# Wed, 16 Nov 2022 05:19:24 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=945c3e29ac7386e00c9eeeb2a5ccc836acb0ce9883fbc29df82fd41c90eb3bd6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=746c3e134598341d1d71680725eb9289a402c6621cae55ae48758e0bad3f7849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b279454d8e2827800b18b736d745126c8d99ffffdcc752156145a6ed5a39cf62;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03b8e4e6a96d6866ce3d69c88770a77a9cb01515ea6b01be8c2e915315bf3bc`  
		Last Modified: Wed, 16 Nov 2022 05:20:14 GMT  
		Size: 45.1 MB (45074595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c205655d2ddc506febbf0c65feb57397b205ce0d3a1f66909ecba8cbc789569`  
		Last Modified: Wed, 16 Nov 2022 05:20:07 GMT  
		Size: 2.2 MB (2162034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf4b062abb4678afe2cac48a89f602c47afd7a64c3475f49237496133952033`  
		Last Modified: Wed, 16 Nov 2022 05:20:34 GMT  
		Size: 193.3 MB (193289116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:1eb86928c9e0b6ca340446b722553c22e58d5c16753715b27dfdc6b129b2af4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180597344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0746f51fbb34ea43bddca9b5753599facc2bd488761d1f06941a6de18a9aa8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:33:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:33:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 15 Nov 2022 12:33:12 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 15 Nov 2022 12:33:12 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 12:33:12 GMT
WORKDIR /root
# Tue, 15 Nov 2022 12:33:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=945c3e29ac7386e00c9eeeb2a5ccc836acb0ce9883fbc29df82fd41c90eb3bd6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=746c3e134598341d1d71680725eb9289a402c6621cae55ae48758e0bad3f7849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b279454d8e2827800b18b736d745126c8d99ffffdcc752156145a6ed5a39cf62;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a060836b3eca611673ccd9d680e368afe1b43c4cca5c29daf2bf9ff5b11458`  
		Last Modified: Tue, 15 Nov 2022 12:34:41 GMT  
		Size: 41.0 MB (40956512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e54b8a06fcdc482f156780c911fc2d95e08e631c0b957a399dcc73e6628671`  
		Last Modified: Tue, 15 Nov 2022 12:34:34 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193fefa5d2e13fc8de0bfac64c0ed533357f93eec7e96dd86e901ad1500ccf80`  
		Last Modified: Tue, 15 Nov 2022 12:34:55 GMT  
		Size: 111.8 MB (111776122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:ba94e46c5b803d309a5ab5e4618ce0fdb330100ccc5604509c252be5a4a6e885
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189555289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:314b8c9d8315d036a02ca87758026d1dbe6047df1970d43c39e30fc86b4616ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:11:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:11:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 15 Nov 2022 06:11:05 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 15 Nov 2022 06:11:05 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 06:11:05 GMT
WORKDIR /root
# Tue, 15 Nov 2022 06:11:11 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=945c3e29ac7386e00c9eeeb2a5ccc836acb0ce9883fbc29df82fd41c90eb3bd6;             SDK_ARCH="x64";;         armhf)             DART_SHA256=746c3e134598341d1d71680725eb9289a402c6621cae55ae48758e0bad3f7849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=b279454d8e2827800b18b736d745126c8d99ffffdcc752156145a6ed5a39cf62;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3729c0d5ddd23a699e7ae39f70e9e06b60350a32241193af26e44db304209b8`  
		Last Modified: Tue, 15 Nov 2022 06:11:53 GMT  
		Size: 45.0 MB (44996105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf6b051280d052da0a85d4d91ee2188ff667504db0e1014876b1d2bcc6d38f`  
		Last Modified: Tue, 15 Nov 2022 06:11:48 GMT  
		Size: 1.6 MB (1562186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061cd9671865bcdce21892a8c84bd79f5cd81b59400cb308467474dd71d8ca7a`  
		Last Modified: Tue, 15 Nov 2022 06:12:00 GMT  
		Size: 112.9 MB (112936393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
