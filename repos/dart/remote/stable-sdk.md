## `dart:stable-sdk`

```console
$ docker pull dart@sha256:486c7ba145a3c9ce8a10d31823c40b34e732276c5105ec4991a4cf9bf68f0068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d90c897bf4d29dcfdabc37bc69ba58ca08f82b20b4e35cda03d0d3a652ada5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271933602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c097fa699aa8fb0f73fc9484d83dd2fb0f21efd5c950e25ee0f5f0f1d9880f38`
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
# Tue, 30 Aug 2022 18:19:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e391c4ed8f623b9748f897cb585d629057c1141f9eaf8e9b2be118932ba11632;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2e83b4a03a9210713a2c65d2c50bd680984c414c3c89d78baba5a20f378fac7d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=06dd7c6eb6c903f5df8b23f9a35f7b1c35ccb869be6b5019c7dd93868ae2bfbf;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:321607f3bacc20609519348edb734a9b87c5a5f8a4a805de16bfcd50134e9fa8`  
		Last Modified: Tue, 30 Aug 2022 18:20:31 GMT  
		Size: 193.3 MB (193336576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:7735323be76e625dff520fe48525ab32bb54e4a30c4982aad310f6d61688717d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180579219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486e81d935d9c87269922ac9da53563e2c7f22f3fe659d0bf4cd19857f52dea5`
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
# Tue, 30 Aug 2022 18:57:31 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e391c4ed8f623b9748f897cb585d629057c1141f9eaf8e9b2be118932ba11632;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2e83b4a03a9210713a2c65d2c50bd680984c414c3c89d78baba5a20f378fac7d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=06dd7c6eb6c903f5df8b23f9a35f7b1c35ccb869be6b5019c7dd93868ae2bfbf;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:f61bf9e23c1408cf4022c995ea389a12cb5defd1608fd810b87ee63023ca9bad`  
		Last Modified: Tue, 30 Aug 2022 18:58:30 GMT  
		Size: 111.8 MB (111755295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:8b1dc8034d049acccd07ac70e8804c5309a2b9cae00030d83a889e54875ca314
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189343817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dddd9c91b788009487c5bf0ec6d8f8d5954ecf4ffdf6b36d563d5a9a0e00f1d`
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
# Tue, 30 Aug 2022 18:39:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=e391c4ed8f623b9748f897cb585d629057c1141f9eaf8e9b2be118932ba11632;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2e83b4a03a9210713a2c65d2c50bd680984c414c3c89d78baba5a20f378fac7d;             SDK_ARCH="arm";;         arm64)             DART_SHA256=06dd7c6eb6c903f5df8b23f9a35f7b1c35ccb869be6b5019c7dd93868ae2bfbf;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:ad732c5c6eba094e1a44ab7ec9a4a203b3e1590d4e2486b68dd8e27686fafd48`  
		Last Modified: Tue, 30 Aug 2022 18:40:35 GMT  
		Size: 112.9 MB (112924877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
