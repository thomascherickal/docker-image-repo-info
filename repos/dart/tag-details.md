<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.13`](#dart213)
-	[`dart:2.13-sdk`](#dart213-sdk)
-	[`dart:2.13.1`](#dart2131)
-	[`dart:2.13.1-sdk`](#dart2131-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13-sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.1`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13.1` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.1-sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:2.13.1-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:76d0bf1a79e33bd6e104275aba3d8a1e8479705323ec0e8b00ced40616024c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6fcb56b6a0d0e4cb4a0ac42a471e1b05811c2be8275a2be86e4fb18c817e3509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.0 MB (248985544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d5235c6c4252be8f4b80f9aef334ecd0e2a9ecd43348dbb0fb3223daddb93`
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
# Tue, 25 May 2021 21:19:43 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.1/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "384b936b2033f9d57b94b2fae86202ba362bc5df811b5d98e401f0ec9fe5087f *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
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
	-	`sha256:61b8754f37255b981ad8d8588b832eeeadf33da3c4ee9785bd20b8f216143528`  
		Last Modified: Tue, 25 May 2021 21:20:30 GMT  
		Size: 195.8 MB (195797599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
