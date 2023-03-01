## `dart:stable-sdk`

```console
$ docker pull dart@sha256:0a026627a5ffeaa20907bba6ace9e42585720a34771efef5c1ee622ae8ebbd32
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
$ docker pull dart@sha256:fca308320a95954cf54d54e95ff1325c037e95b909d4591e8b639f341e6c39e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205965262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adcfa1c1e50e57e6ee8608dfcd24327022882b57e67d85aca7f89bb24bf8e93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:39:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:39:11 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 09 Feb 2023 09:39:11 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 09 Feb 2023 09:39:11 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:39:11 GMT
WORKDIR /root
# Thu, 09 Feb 2023 09:39:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=326f6085aaf3a6733f3cf2eface18513afbd07c70e4068c4da9c6880161ddb2b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=d3fddaabce691a316a2e3eb8c51f2bd46f53f073cf0e38b525cfc404f0a0d72c;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4c6f5139bde79f557af92790d219e64f1a2e043a657848e5618efbcb82f9b77e;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.2/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81568e60ca7407142c1889fea5a3e1aebc8486fe202a5eb3c39534c594c6ac`  
		Last Modified: Thu, 09 Feb 2023 09:39:49 GMT  
		Size: 45.0 MB (45009126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41da113f835130b90931baea94afb088901395397be57f6739d97bf0fa0297fe`  
		Last Modified: Thu, 09 Feb 2023 09:39:44 GMT  
		Size: 1.6 MB (1562178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df0f0a89d057da80d217dc4fe2a08826632e8a3ab108426efe3995d0a361cba`  
		Last Modified: Thu, 09 Feb 2023 09:39:59 GMT  
		Size: 129.3 MB (129331449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
