## `dart:2-sdk`

```console
$ docker pull dart@sha256:a0bd588eb8f4d4242cbcdfccb6d1c3b5eb3498ad0c18549377f7a81348d39245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:cb12803ba785bc96cc7a6df6fed93aa77fea327379f624995b285cb7126beca2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275827174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d020e798376619845439ed6c2244245bfcf12a70746ff007a4209f2ea5c76336`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:02:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:02:51 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 Aug 2022 01:02:52 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 Aug 2022 01:02:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 01:02:52 GMT
WORKDIR /root
# Thu, 25 Aug 2022 18:22:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=ba8bc85883e38709351f78c527cbf72e22cd234b3678a1ec6a2e781f7984e624;             SDK_ARCH="x64";;         armhf)             DART_SHA256=701de8f09d92abadbee8773828c40f52a173fe5eae378d3bf84fd6becb9242f4;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ee0acf66e184629b69943e9f29459e586095895c6aae6677ab027d99c00934b6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb560d52a31acbd32a4f357b69ca8a95b39c44794c8288e569a2843a7abdadd`  
		Last Modified: Tue, 23 Aug 2022 01:03:49 GMT  
		Size: 45.1 MB (45075989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fc341668ed4edfe9e06de856dffd63709856fad6a289de2992c44997673876`  
		Last Modified: Tue, 23 Aug 2022 01:03:42 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152b45a493143d1b022def70962fe6ba57307a098c488438d391cc65915d44dc`  
		Last Modified: Thu, 25 Aug 2022 18:23:20 GMT  
		Size: 197.2 MB (197230148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:9de2c1595f91597575799174ea89cc0e08e016e3953adce62b24731b00b260e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184081946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc50157a5fab13449ff5487fc4ce8cffa0589dd4a79f330a87ddac35d46f382`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:17:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:17:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 Aug 2022 13:17:32 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 Aug 2022 13:17:32 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 13:17:32 GMT
WORKDIR /root
# Tue, 23 Aug 2022 13:17:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f837f385603a1cfb14ddb7dd0cd64820b297646626bdb689ccfc3278fa83b2b1;             SDK_ARCH="x64";;         armhf)             DART_SHA256=3eae7ed5773c125165d123a235bac9956981cfdf164059806ed69a6feefc1eda;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8e71b0c958a587c83ecd6c8cc637bc624bb85bc64e877e9ea00831a659a904b1;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a68fbe45d541e5e1d8b1b158629e3f1632bcc00f41399c7b02f46ec9b48a521`  
		Last Modified: Tue, 23 Aug 2022 13:19:05 GMT  
		Size: 41.0 MB (40964111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344f92898b62ae8bfa9992220ebaeaa2cf1866d7373ecd2e7443d84768910168`  
		Last Modified: Tue, 23 Aug 2022 13:18:52 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d7b673ee491833c3eacc45ed01c065d9f51a8f6f52a482909e7f425c90e3f6`  
		Last Modified: Tue, 23 Aug 2022 13:19:21 GMT  
		Size: 115.3 MB (115258022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:b6f2b94d06dcaba1f353f5b312dc6cdbda0de337fb8a95bf00bf914257a340d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193153859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f87969fea6ab007563f9e812865c4857d93309b9e7020f360c650ffa792b2ec0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:45:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:45:11 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 23 Aug 2022 02:45:12 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 23 Aug 2022 02:45:13 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 02:45:14 GMT
WORKDIR /root
# Thu, 25 Aug 2022 18:40:12 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=ba8bc85883e38709351f78c527cbf72e22cd234b3678a1ec6a2e781f7984e624;             SDK_ARCH="x64";;         armhf)             DART_SHA256=701de8f09d92abadbee8773828c40f52a173fe5eae378d3bf84fd6becb9242f4;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ee0acf66e184629b69943e9f29459e586095895c6aae6677ab027d99c00934b6;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.17.7/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c70daf8007713a8a9d33c825885754e7cfa4c68eec5ea6a5c402777d0b9a80b`  
		Last Modified: Tue, 23 Aug 2022 02:46:22 GMT  
		Size: 44.8 MB (44798419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3456734c399cd46ed73bdaec58c27712844f78746f5e9561939cdf1a330f31`  
		Last Modified: Tue, 23 Aug 2022 02:46:16 GMT  
		Size: 1.6 MB (1556733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d7ad12b0746cae21dd265191ac2f5c3f63d007e0c9714389309e9b9f89bda0`  
		Last Modified: Thu, 25 Aug 2022 18:41:20 GMT  
		Size: 116.7 MB (116734919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
