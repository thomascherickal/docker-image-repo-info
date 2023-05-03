## `dart:stable-sdk`

```console
$ docker pull dart@sha256:fce7449adeaebfde14485bde42867de7fdbce0a45eacacc06c1c97d9f4f9c15e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:4f1928e0b716f4b64fac8258140b4146691dee53b3dcc17feee7374d8a225241
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300608861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d4b6f1b0e9d39ae132ee146f738a1c0a590a7810007fc0aa6ee7e5250545faf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:33:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:33:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 12 Apr 2023 08:33:29 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 12 Apr 2023 08:33:30 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:33:30 GMT
WORKDIR /root
# Wed, 12 Apr 2023 08:33:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0fdff25e6acba3d6094155a7e341634f8de3477e86c2fda4ad47232c1adf704f;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7286b3a935c98ec9731c6e540614ef20e8ad8a1d6bef194c79e29d9837363de3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=6913b7c0b3b78bc141d372cd473da21771e57372b1ab45c977ce1550c8ff0b9c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e52eb76fdb91cbc25711f2ba984c87a3be0642c4f328728d8c68e5cfdc39bf4`  
		Last Modified: Wed, 12 Apr 2023 08:34:26 GMT  
		Size: 45.1 MB (45101893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc2e823c2e74845a6e9ece7319b00d4a722a0921a626fcd2e9f9cc0e7e53f65`  
		Last Modified: Wed, 12 Apr 2023 08:34:19 GMT  
		Size: 2.2 MB (2162030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f875f67c3e4664b1fb80756ea1a35ebc5eeb498164129098251919b3271ff5e`  
		Last Modified: Wed, 12 Apr 2023 08:34:49 GMT  
		Size: 221.9 MB (221926710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:034084bf670ed904a16c17302d212d2033c2720638db5bc53e5a5ccb3f9cb0cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196761141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb50065e507ddff140adfd4e42cff4137b55738c5091bd9a313e28e865a38776`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:13:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:13:21 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 12 Apr 2023 08:13:21 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 12 Apr 2023 08:13:21 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:13:21 GMT
WORKDIR /root
# Wed, 12 Apr 2023 08:13:37 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0fdff25e6acba3d6094155a7e341634f8de3477e86c2fda4ad47232c1adf704f;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7286b3a935c98ec9731c6e540614ef20e8ad8a1d6bef194c79e29d9837363de3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=6913b7c0b3b78bc141d372cd473da21771e57372b1ab45c977ce1550c8ff0b9c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3be026e596ed1d8caab8137e502a98f853ee0a637a08328e101868822bdc71`  
		Last Modified: Wed, 12 Apr 2023 08:14:22 GMT  
		Size: 41.0 MB (40988814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc39dc8920f9c9b88f8d00e1616d1cec5e94911e3b89dbc171a83bfec09d70d`  
		Last Modified: Wed, 12 Apr 2023 08:14:16 GMT  
		Size: 1.3 MB (1288550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47235f02f1d1f8f554b45f5f70dbe32876968f76c8556a65618840588ac43e3b`  
		Last Modified: Wed, 12 Apr 2023 08:14:40 GMT  
		Size: 127.9 MB (127904005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:70740db9149f0456e07c23852ae990dbf21ab9f34cab65126ef67c5a10becfc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205977515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe885d6a8170f1ce8f45dcb811539c2d0220ee9900a72b833264c5ae78b0f9a0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:01:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:01:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 03 May 2023 18:01:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 03 May 2023 18:01:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 18:01:44 GMT
WORKDIR /root
# Wed, 03 May 2023 18:01:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0fdff25e6acba3d6094155a7e341634f8de3477e86c2fda4ad47232c1adf704f;             SDK_ARCH="x64";;         armhf)             DART_SHA256=7286b3a935c98ec9731c6e540614ef20e8ad8a1d6bef194c79e29d9837363de3;             SDK_ARCH="arm";;         arm64)             DART_SHA256=6913b7c0b3b78bc141d372cd473da21771e57372b1ab45c977ce1550c8ff0b9c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fc0b14711e98b08b1a032b2deb48049f18fd73081b8c279a065a4c3d917122`  
		Last Modified: Wed, 03 May 2023 18:02:26 GMT  
		Size: 45.0 MB (45011139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28e1fa58a15ccb7cc2d05484fac11f66090b0c7d8833a0193a8c9c036c8e171`  
		Last Modified: Wed, 03 May 2023 18:02:22 GMT  
		Size: 1.6 MB (1560886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4360e393242fd8893b744aea8fe841b075de8e50467c1a8f590342451e8a886b`  
		Last Modified: Wed, 03 May 2023 18:02:36 GMT  
		Size: 129.4 MB (129352757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
