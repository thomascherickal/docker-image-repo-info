## `dart:beta`

```console
$ docker pull dart@sha256:6291b52a1a896ee875d9eb7704304740f90801c6ca84672d5d7fa6b08a80a3cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:2ecd9a092a6939c31387227deb82aafc7f36fad6613a338e3ce1b6c37988b1f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278285286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25e2ffb1d24da071ef7e0b3e220a808077a5b9a30e47f467c2a755271b76212`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 07:14:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 07:14:05 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Fri, 18 Mar 2022 07:14:06 GMT
ENV DART_SDK=/usr/lib/dart
# Fri, 18 Mar 2022 07:14:06 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 07:14:06 GMT
WORKDIR /root
# Fri, 18 Mar 2022 07:14:39 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=edca0fe2afb7cb2a5d6c1ebc65cc9cf92db50940cad452de8ff0040272fe4444;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5a6a93f26d38037c5de99f4b6dc6d9b61d30409f6e405e1704db337a4514e8ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4bb7866c4fdda23e3d9603b27b3c669376b3740b7b9eca2feb8e9ccbc1673bb8;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de649e52a496ec9282231d3f84450e7538888982e435264a68c49a52a3bf28c`  
		Last Modified: Fri, 18 Mar 2022 07:15:08 GMT  
		Size: 45.1 MB (45073507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570b9440ed7963445a41b94a53617cd26c514c3c57a9e0405cf4f59895fd10c2`  
		Last Modified: Fri, 18 Mar 2022 07:15:01 GMT  
		Size: 2.1 MB (2139229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36ef761fdae49f597b014402feb095c156f976ffcf659fa8ddb39a2428acd5`  
		Last Modified: Fri, 18 Mar 2022 07:16:41 GMT  
		Size: 199.7 MB (199695978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:d8256e50a84678c79fd5ac1e64715dc1981e6cf6486347fd4a7cd9aec146dfc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186839876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488a8ebcb1b692cf1aed456f375782d36fd93dc9c98797872f036f593cd99d2a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 04:06:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 04:06:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Sat, 19 Mar 2022 04:06:20 GMT
ENV DART_SDK=/usr/lib/dart
# Sat, 19 Mar 2022 04:06:21 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 04:06:21 GMT
WORKDIR /root
# Sat, 19 Mar 2022 04:07:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=edca0fe2afb7cb2a5d6c1ebc65cc9cf92db50940cad452de8ff0040272fe4444;             SDK_ARCH="x64";;         armhf)             DART_SHA256=5a6a93f26d38037c5de99f4b6dc6d9b61d30409f6e405e1704db337a4514e8ca;             SDK_ARCH="arm";;         arm64)             DART_SHA256=4bb7866c4fdda23e3d9603b27b3c669376b3740b7b9eca2feb8e9ccbc1673bb8;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-182.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f50a925c6c645b6ef53736223c4843dc0f03738c5d47cfebd0f337c39159938`  
		Last Modified: Sat, 19 Mar 2022 04:08:57 GMT  
		Size: 41.0 MB (40965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7005eee92ed88cffe125039e5a8583ee00730058d75deb313299910e2790ed4`  
		Last Modified: Sat, 19 Mar 2022 04:08:33 GMT  
		Size: 1.3 MB (1287889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e5361c3367fde99d33ebaa48b1c2d872061f85bc8f6324d71030b408ccc853`  
		Last Modified: Sat, 19 Mar 2022 04:11:49 GMT  
		Size: 118.0 MB (118011264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:86c036242f0551acd694a8160abbdc60f666c48043246d276f681516b2170441
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195095071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355ee1242b7f1dbceccd165bd615dcca0d017eddadc57a0695d127b2c198e2ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:34:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 17 Mar 2022 22:34:18 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 17 Mar 2022 22:34:19 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 22:34:20 GMT
WORKDIR /root
# Thu, 17 Mar 2022 22:34:47 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=5896bc9fd8543b419870ced8b504b8f33b16c0a0bcf566f3e419e3b35db21006;             SDK_ARCH="x64";;         armhf)             DART_SHA256=56da37cea8b4bc70b17cf08e1b582dcd35392c3611140cda04dcba34bdd4b2ba;             SDK_ARCH="arm";;         arm64)             DART_SHA256=ff5ab6b960a5511eef506236ff5e4b4d115f2786393b59d615c3a0fc242b0639;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-69.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f03fd2f7cd6528e81a11d80a13956cf986e23833cc1e9048d65f9b07738171`  
		Last Modified: Thu, 17 Mar 2022 22:35:28 GMT  
		Size: 44.8 MB (44789139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222cbf5294e357d83725e3729c0c0f883cbf0920d388ad9ed7871c4f1f237ee4`  
		Last Modified: Thu, 17 Mar 2022 22:35:21 GMT  
		Size: 1.6 MB (1556530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4892c372ece4b0611bfb1b78ffdcd4916e99f1d5f4f3fa9840378ac195eb66`  
		Last Modified: Thu, 17 Mar 2022 22:36:30 GMT  
		Size: 118.7 MB (118686389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
