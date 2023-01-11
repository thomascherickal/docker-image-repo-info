## `dart:stable`

```console
$ docker pull dart@sha256:33caaa23adc28949959517733f989e86f077ea6dee825d543685df1fcf5d57f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:4bb4e1e68f352be7bb5e7a4ed8be71d37b37240123da9d398c0b7f66c8f639e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271928525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2879bae8422cb66e93fb61d8998480cea7870ce35ea01ccabc488b776601e4cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:45:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:45:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 03:45:52 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 03:45:52 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:52 GMT
WORKDIR /root
# Wed, 11 Jan 2023 03:46:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=492c0e835203c4402e3d8291d12b53927f0300c8080aaf63a9113c204255a735;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c360ff64d1306ed5038a7df98142eff832abebc486d3e2b7f68b0fc53279a849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=61dbb462b48aee4f3184b6ecdd356632f39165ae8570fe77a62900a6444f702c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6ceb6bff25bb7e23c1f0241699fd427a735539dd70213495fdf8b34ed5b5e`  
		Last Modified: Wed, 11 Jan 2023 03:46:55 GMT  
		Size: 45.1 MB (45073156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148029c06d512bfa87f2ff720f96e037b633b3e80b2f16e076402d4049cfdd2`  
		Last Modified: Wed, 11 Jan 2023 03:46:48 GMT  
		Size: 2.2 MB (2162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e87a18cfbb698646def498f6d18174e81396e4f3a799ed25d3fed0f79ce5c20`  
		Last Modified: Wed, 11 Jan 2023 03:47:16 GMT  
		Size: 193.3 MB (193296362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:dd1bc4a9fb90ba6c7f70d3f02bc7c3a5c4e446a8e308c43712b37aea6d9dd699
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180589866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54601ff6b338a6b1b9c1ad218cd82e5f1b571e58c86c18f45a7c6d411307fb0b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:52:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:52:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:52:03 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:52:03 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:52:03 GMT
WORKDIR /root
# Wed, 11 Jan 2023 04:52:13 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=492c0e835203c4402e3d8291d12b53927f0300c8080aaf63a9113c204255a735;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c360ff64d1306ed5038a7df98142eff832abebc486d3e2b7f68b0fc53279a849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=61dbb462b48aee4f3184b6ecdd356632f39165ae8570fe77a62900a6444f702c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ef8a6fd94f64d59b6e1945dd639fdf419e73ac8677087bce3b4481d1e740b`  
		Last Modified: Wed, 11 Jan 2023 04:53:24 GMT  
		Size: 41.0 MB (40955530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d817971bc698f81b85279e3b7aabc2fb1f2acd97c7d29661d79c1a5aa0605733`  
		Last Modified: Wed, 11 Jan 2023 04:53:17 GMT  
		Size: 1.3 MB (1288515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf40cc7eda8ff826e733983b044d8c4de92db2440181b099569d487db9abc92`  
		Last Modified: Wed, 11 Jan 2023 04:53:38 GMT  
		Size: 111.8 MB (111786333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:23be05afb20bba5eabb877f901af44133f6c8cc996709c6f45f5a238ae82ea79
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189542501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6519298360ac1919bfb7bb9d6e7baf3a31dde61dad730efb7cd235f7a71281a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:00:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:00:44 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Jan 2023 04:00:44 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Jan 2023 04:00:44 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 04:00:44 GMT
WORKDIR /root
# Wed, 11 Jan 2023 04:00:52 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=492c0e835203c4402e3d8291d12b53927f0300c8080aaf63a9113c204255a735;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c360ff64d1306ed5038a7df98142eff832abebc486d3e2b7f68b0fc53279a849;             SDK_ARCH="arm";;         arm64)             DART_SHA256=61dbb462b48aee4f3184b6ecdd356632f39165ae8570fe77a62900a6444f702c;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.6/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2814cdd6986e359cfa22f10d27bdd8c5b227c76d42f20c99a2f4c9bb4dc3b75`  
		Last Modified: Wed, 11 Jan 2023 04:01:35 GMT  
		Size: 45.0 MB (44994736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2faa032a88fd1e7feba61ef9aaac09529900a286c643beeea0e5e2a1c53816`  
		Last Modified: Wed, 11 Jan 2023 04:01:30 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887c58fa32cc963fa40e4711494d5000252e5bc5d435717a470b6b2a9eb4d4bb`  
		Last Modified: Wed, 11 Jan 2023 04:01:43 GMT  
		Size: 112.9 MB (112940767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
