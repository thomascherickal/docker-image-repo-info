<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.13`](#dart213)
-	[`dart:2.13-sdk`](#dart213-sdk)
-	[`dart:2.13.4`](#dart2134)
-	[`dart:2.13.4-sdk`](#dart2134-sdk)
-	[`dart:2.14.0-377.4.beta`](#dart2140-3774beta)
-	[`dart:2.14.0-377.4.beta-sdk`](#dart2140-3774beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.13` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13-sdk`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.13-sdk` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.4`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.13.4` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.13.4-sdk`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:2.13.4-sdk` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.14.0-377.4.beta`

```console
$ docker pull dart@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `dart:2.14.0-377.4.beta-sdk`

```console
$ docker pull dart@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `dart:beta`

```console
$ docker pull dart@sha256:61e57d192bfb4b7fb24c81bc686a7d6d8d488b4819c7caa8517b32b8e95f953e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:f6d161ce735b2593daf2fcaf8ebe3841f4cbcdda163818b9e88fa23f0c15962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288872732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2914b2f1e8d3ac60e3b867f455238c2113906613edcb07e8a17976b378304162`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:27:08 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.14.0-188.5.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "11c2e3a35e0a13de20e5d88831db69bd7d18c077b10c77cbabd61dc36e473ba7 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c542c6f23450787b0256b13feb611914bff841bac6a0b2bc8f66ce98aa79025`  
		Last Modified: Thu, 22 Jul 2021 01:29:26 GMT  
		Size: 209.8 MB (209786553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:61e57d192bfb4b7fb24c81bc686a7d6d8d488b4819c7caa8517b32b8e95f953e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:f6d161ce735b2593daf2fcaf8ebe3841f4cbcdda163818b9e88fa23f0c15962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288872732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2914b2f1e8d3ac60e3b867f455238c2113906613edcb07e8a17976b378304162`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:27:08 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.14.0-188.5.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "11c2e3a35e0a13de20e5d88831db69bd7d18c077b10c77cbabd61dc36e473ba7 *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c542c6f23450787b0256b13feb611914bff841bac6a0b2bc8f66ce98aa79025`  
		Last Modified: Thu, 22 Jul 2021 01:29:26 GMT  
		Size: 209.8 MB (209786553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:8db1f439a736cff8651f7be9963fc2449fb52d53c1cb17b00db41414fded6c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:79214ba7cfc42d99e826bdeee39ad9cb1767b47ed0464126af55c96eeb552a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274814139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247d156397d09364096742c403bbf71ec9fd725917dbf8eaa1f0b046d0810aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:26:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:26:39 GMT
RUN set -eux;     for f in         /etc/nsswitch.conf         /etc/ssl/certs         /lib/x86_64-linux-gnu/libc.so.6         /lib/x86_64-linux-gnu/libdl.so.2         /lib/x86_64-linux-gnu/libm.so.6         /lib/x86_64-linux-gnu/libnss_dns.so.2         /lib/x86_64-linux-gnu/libpthread.so.0         /lib/x86_64-linux-gnu/libresolv.so.2         /lib/x86_64-linux-gnu/librt.so.1         /lib64/ld-linux-x86-64.so.2         /usr/share/ca-certificates     ; do         dir="$(dirname "$f")";         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 22 Jul 2021 01:26:39 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 22 Jul 2021 01:26:39 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 01:26:39 GMT
WORKDIR /root
# Thu, 22 Jul 2021 01:26:50 GMT
RUN set -eux;     ARCH=$(case "$(dpkg --print-architecture)" in amd64) echo "x64";; esac;);     SDK="dartsdk-linux-$ARCH-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.13.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "633a9aa4812b725ff587e2bbf16cd5839224cfe05dcd536e1a74804e80fdb4cd *$SDK"     | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK";
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70abda323f089ac700867be815ab89be053cbdc74a0823b9a44fafcd0363153`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 49.6 MB (49581247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af578853d94f554b9fd289dc844a19b103b09b0ffb62f0b872c763dcfd6ec40`  
		Last Modified: Thu, 22 Jul 2021 01:27:33 GMT  
		Size: 2.4 MB (2359137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9eaf2e41c0873f5d25960a497dccb4246b6148309c5e253ec844c406a9f8e3`  
		Last Modified: Thu, 22 Jul 2021 01:28:09 GMT  
		Size: 195.7 MB (195727960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
