<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.13`](#dart213)
-	[`dart:2.13-sdk`](#dart213-sdk)
-	[`dart:2.13.0`](#dart2130)
-	[`dart:2.13.0-sdk`](#dart2130-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13-sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13-sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.0`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13.0` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.0-sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13.0-sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:f894a799697fd0eaba8a6f9a457c9b28781dec0623943d29969f50d9fa0658c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:24458b63ea30997ed4043e3c3c50057993d29abc058481782845eaa3b9229c9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248816151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8054b3dc224a3d039618760c1955d83a9b18f37d045045b6b9f691d66a08b59e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Mon, 17 May 2021 20:18:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         openssh-client         unzip         dnsutils     ;     rm -rf /var/lib/apt/lists/*
# Mon, 17 May 2021 20:18:55 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Mon, 17 May 2021 20:18:55 GMT
ENV DART_SDK=/usr/lib/dart
# Mon, 17 May 2021 20:18:55 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 May 2021 20:18:56 GMT
WORKDIR /root
# Wed, 19 May 2021 19:19:44 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.0/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "4d39fe12ef1fc2f1c98246c1f8482203398eb120f724c0789db8d4b2ffe25362 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6b6cb7d8e58573bab3165075efc383447aaf34b4eff54c220f0ee5b55206f`  
		Last Modified: Mon, 17 May 2021 20:19:57 GMT  
		Size: 23.7 MB (23682897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4bafd8baa9cbcae1f326916610f19c163a88d49af4205c08859fd4631e9a75`  
		Last Modified: Mon, 17 May 2021 20:19:53 GMT  
		Size: 2.4 MB (2359133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b944b395928ffab19ee1a58f2725e4790cdecf70c5a563b38cb1b6bbf20aee`  
		Last Modified: Wed, 19 May 2021 19:20:32 GMT  
		Size: 195.6 MB (195628206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
