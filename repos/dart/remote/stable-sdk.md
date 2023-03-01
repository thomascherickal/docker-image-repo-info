## `dart:stable-sdk`

```console
$ docker pull dart@sha256:9825f5fc2c98206cf8322b487e9c4f072040dfec2b2a8dca5a41983ef5501059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:eb56334362271258437ff9f487399dc2d4c018c649fc75014fb14e78e6e612bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300573924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb7a113a9a982f35b9580722a653562a0b8f6de61c9cecbb9cfbebcabe41bf5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:00:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:00:10 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 01 Mar 2023 05:00:11 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 01 Mar 2023 05:00:11 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 05:00:11 GMT
WORKDIR /root
# Wed, 01 Mar 2023 05:00:25 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=326f6085aaf3a6733f3cf2eface18513afbd07c70e4068c4da9c6880161ddb2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d3fddaabce691a316a2e3eb8c51f2bd46f53f073cf0e38b525cfc404f0a0d72c;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4c6f5139bde79f557af92790d219e64f1a2e043a657848e5618efbcb82f9b77e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc65615115efc0214c3c9c0c85199857a0ddff5901bbc028bfa2dd6156d5fe5`  
		Last Modified: Wed, 01 Mar 2023 05:01:13 GMT  
		Size: 45.1 MB (45101765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcbccd766aa06004906194a9d2e07d3e01d1791d99edf901dda9e0ab3f0b415`  
		Last Modified: Wed, 01 Mar 2023 05:01:06 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa862ef04a0fd0a6d18bb191a273d963b56eccbe7fa9332d4ec75a3f681d9a3e`  
		Last Modified: Wed, 01 Mar 2023 05:01:37 GMT  
		Size: 221.9 MB (221898734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:a2e1de47d6ef7c857b572b97a1de181706f166044a513ad7517808b7b7ee51bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196729756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b652b351493def24998366d5910529ec9ac67bbecca59b573a06aca2304061`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:25:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:25:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 01 Mar 2023 02:25:08 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 01 Mar 2023 02:25:08 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 02:25:08 GMT
WORKDIR /root
# Wed, 01 Mar 2023 02:25:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=326f6085aaf3a6733f3cf2eface18513afbd07c70e4068c4da9c6880161ddb2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d3fddaabce691a316a2e3eb8c51f2bd46f53f073cf0e38b525cfc404f0a0d72c;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4c6f5139bde79f557af92790d219e64f1a2e043a657848e5618efbcb82f9b77e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a2a2202be4ce8d1e3c64eeb5cd1a880b653007a431bebfcb9aa6b27ac927e`  
		Last Modified: Wed, 01 Mar 2023 02:26:29 GMT  
		Size: 41.0 MB (40988626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2c1c5227941118e0a1f640f63b2b993bb7b3e42883849a783c7f7cd6d4487`  
		Last Modified: Wed, 01 Mar 2023 02:26:22 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1267482ac995e36cef41a6ad24235b7d5598f8d2b6ab7959dc3f97ba8d752f`  
		Last Modified: Wed, 01 Mar 2023 02:26:44 GMT  
		Size: 127.9 MB (127875299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e39615b00edefeef8dd3c7c39479ddd6d4219ac9e1b1facb999c2340acf5dc3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205967650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b47ddfdf2c17d6a220429b1d3b9e4c7c103126c167984396f81e8838ddfa9a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:03:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:03:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 01 Mar 2023 13:03:50 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 01 Mar 2023 13:03:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 13:03:50 GMT
WORKDIR /root
# Wed, 01 Mar 2023 13:03:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=326f6085aaf3a6733f3cf2eface18513afbd07c70e4068c4da9c6880161ddb2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d3fddaabce691a316a2e3eb8c51f2bd46f53f073cf0e38b525cfc404f0a0d72c;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4c6f5139bde79f557af92790d219e64f1a2e043a657848e5618efbcb82f9b77e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad58cbb76aa261586e238ac663c806e6da6fda3059b45385c8c3938a59387`  
		Last Modified: Wed, 01 Mar 2023 13:04:43 GMT  
		Size: 45.0 MB (45011137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f122052879f43039ebbbbe28f2f87037e49d388f36058bf9b4f1e579229b1a`  
		Last Modified: Wed, 01 Mar 2023 13:04:38 GMT  
		Size: 1.6 MB (1562174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9aa495704604441c6ba748ce3a53b348ef2cb7838b8e7c082a0c7bb2cf0d56`  
		Last Modified: Wed, 01 Mar 2023 13:04:53 GMT  
		Size: 129.3 MB (129331525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
