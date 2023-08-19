## `dart:stable-sdk`

```console
$ docker pull dart@sha256:96d2e5d03b8356c2a7542716ace7dce745971efe1d03888a1d7ecd2e7c1dde36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6074ac9e222bf68d7a481acf8e5b25353122e0255cb0ba7d96bc602fa9eece02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291218660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2ccb38bd4255ded8d76a37e72a7c1fda5e13c378beecd543d20b72981c27c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:21:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 07:21:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 16 Aug 2023 07:21:32 GMT
ENV DART_SDK=/usr/lib/dart
# Fri, 18 Aug 2023 23:19:26 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Aug 2023 23:19:26 GMT
WORKDIR /root
# Fri, 18 Aug 2023 23:19:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7ce5c1560b1d8ea5ee0e6d44f1c3e7b804ddc5377b38d72fe4d43009a6c67e84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ac5880e17b80e046d59eeac46a77d084a8937804dd4a4564a26c53d453df890f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=fd4fcc05f1d1c82fd618b83c7d877968460c5bd425774d89add438be12a20795;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2577ff5100d24131ef5c0b1d5abb88623898588a87bafbed311deab71d09ee`  
		Last Modified: Wed, 16 Aug 2023 07:22:28 GMT  
		Size: 45.1 MB (45101830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4d59ba3d1a7503ca685749da21497c47644df01b1409c1ce14a6d494fd9436`  
		Last Modified: Wed, 16 Aug 2023 07:22:22 GMT  
		Size: 2.2 MB (2160697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b502cc2bfaf72b519f73f76b703913c7b35ea7f17e6dd187ee73648076ffe36c`  
		Last Modified: Fri, 18 Aug 2023 23:20:45 GMT  
		Size: 212.5 MB (212538455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:c5ea518570e61bc857a759789f90bbce34f29bbd194f224059bc7f7ff1e1d8c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182227551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca3b186e35ed9d4697ae0fa3f266c94cfe431085824aa5fd260f29325150680`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:00:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:00:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 16 Aug 2023 15:00:35 GMT
ENV DART_SDK=/usr/lib/dart
# Fri, 18 Aug 2023 23:57:17 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Aug 2023 23:57:18 GMT
WORKDIR /root
# Fri, 18 Aug 2023 23:57:27 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7ce5c1560b1d8ea5ee0e6d44f1c3e7b804ddc5377b38d72fe4d43009a6c67e84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ac5880e17b80e046d59eeac46a77d084a8937804dd4a4564a26c53d453df890f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=fd4fcc05f1d1c82fd618b83c7d877968460c5bd425774d89add438be12a20795;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9550e27958af98a4d93dc3dbcd1edcfafd99d14de8df8b555d57510383ce97a`  
		Last Modified: Wed, 16 Aug 2023 15:01:37 GMT  
		Size: 41.0 MB (40988435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555b973d8367ff0c896fa7540e845348f6d8f5dd0136861e82f831ccf4384b81`  
		Last Modified: Wed, 16 Aug 2023 15:01:28 GMT  
		Size: 1.3 MB (1287722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593faba3c6c04f7bb5ea007ea4a8dbd2d5c26ecf90de9567cf80d93b3dc8452`  
		Last Modified: Fri, 18 Aug 2023 23:58:17 GMT  
		Size: 113.4 MB (113372757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e9e8971464846b485058a4e516cb99abe53317cb3cb840404458d4560014e4ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191391237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4900465f2d5f88b3c7598b2efed3f06568364108174502fcbb4dc2cb95787300`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:02:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:18 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 16 Aug 2023 02:02:18 GMT
ENV DART_SDK=/usr/lib/dart
# Fri, 18 Aug 2023 23:39:25 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Aug 2023 23:39:25 GMT
WORKDIR /root
# Fri, 18 Aug 2023 23:39:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=7ce5c1560b1d8ea5ee0e6d44f1c3e7b804ddc5377b38d72fe4d43009a6c67e84;             SDK_ARCH="x64";;         armhf)             DART_SHA256=ac5880e17b80e046d59eeac46a77d084a8937804dd4a4564a26c53d453df890f;             SDK_ARCH="arm";;         arm64)             DART_SHA256=fd4fcc05f1d1c82fd618b83c7d877968460c5bd425774d89add438be12a20795;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c88ee4e2ded4b674611c7a0cc207fa18d0c207f6898b4c4a97598b60dc687d3`  
		Last Modified: Wed, 16 Aug 2023 02:03:00 GMT  
		Size: 45.0 MB (45011889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f4393bc25a5d3316c200e692678aa19db82688e7b1d5442111eecc8273919`  
		Last Modified: Wed, 16 Aug 2023 02:02:55 GMT  
		Size: 1.6 MB (1560880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adff3635333bbe0edc6f75602b086ebcaf856c38a7c5ee50b65408af934a338`  
		Last Modified: Fri, 18 Aug 2023 23:40:16 GMT  
		Size: 114.8 MB (114755652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
