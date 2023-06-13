## `dart:beta`

```console
$ docker pull dart@sha256:d19a5c7453c9ff7f977dfc6956a1a61042386c5572a4dcc249c5b3705b10d41f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:e987a41aae1b7f5ea6667118208c9549087c0d028d9209c5a528000e8051f724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286753987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5536218121a2a670077d1116caaafbfdbb011ae6e3c29b4c13b7e87b3d3f08`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:53:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:53:45 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:53:45 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:53:45 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:53:45 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:54:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c233b919d87b3f40c5d951de404991a8488b089084c10bc959a33b82e4bd08`  
		Last Modified: Tue, 13 Jun 2023 05:54:42 GMT  
		Size: 45.1 MB (45102701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05e2d8750b89e4a469a43dbef8db3d37a0b050d1a927f8725198ee6e84d7c5`  
		Last Modified: Tue, 13 Jun 2023 05:54:36 GMT  
		Size: 2.2 MB (2160701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11a9fc3b7634c5450c15b0eefc87d1320c26447a95e3846eae56f3c87926a7`  
		Last Modified: Tue, 13 Jun 2023 05:55:51 GMT  
		Size: 208.1 MB (208073175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:63ea9264b1ca6c2cef0e0c02d39ee33025eb2a9b4e8f57686e828797b168d6c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178838202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526d6968942b3503534395bef7f3293e07ce0df64cc5852c9f8905b5296370e9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:14:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:14:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 17:14:43 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 17:14:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 17:14:43 GMT
WORKDIR /root
# Tue, 13 Jun 2023 17:15:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede1c8042537f06a8eb323db8c1c90f46560fa30481410c52f734b072861f8c`  
		Last Modified: Tue, 13 Jun 2023 17:15:30 GMT  
		Size: 41.0 MB (40988238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208d562f337083bb0b59f8cd502b83dc4c3f2ce5f5ea7355c6b72c28c6c43c7`  
		Last Modified: Tue, 13 Jun 2023 17:15:24 GMT  
		Size: 1.3 MB (1287728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636ef33cd0c2ee7f69cb84c396778847763187978013fa8b875a29e3699aa2`  
		Last Modified: Tue, 13 Jun 2023 17:16:22 GMT  
		Size: 110.0 MB (109983546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:f7cd4aa6a158304d6967436c0da05657098ff42b0990a4ddbb3fc47724a73b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (187986888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c185c862462a854b1b115e512428873b02cb5ca7184426a571adf52e02726a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:29:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:30:00 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 13 Jun 2023 05:30:00 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 13 Jun 2023 05:30:00 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:30:00 GMT
WORKDIR /root
# Tue, 13 Jun 2023 05:30:23 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=b4d251e51da2b963eae82136b37b83a050f175be82fc8d691b609cb8e030c13b;             SDK_ARCH="x64";;         armhf)             DART_SHA256=32dddc5047f58a3d2b53b0f238aeaf9d951fc7d91559b024fd0e1ca3e0afeaf0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8c65c833fe84010670066450a404e81a9ee311b14cf560e8d6325fc9a351f8b4;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.1.0-163.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a146bde7cf65ec5671588bf160d4ecd4717777c92efb188fe310b02d51f29`  
		Last Modified: Tue, 13 Jun 2023 05:30:41 GMT  
		Size: 45.0 MB (45011234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e0d9b46fabee49930e4019ec81e22dc3905e29d9182a451285ed29ddba2d1`  
		Last Modified: Tue, 13 Jun 2023 05:30:36 GMT  
		Size: 1.6 MB (1560875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036117dbabdbdd829e1fc19eeeb32595f45984c0f9867fb037f5efb42b3d1967`  
		Last Modified: Tue, 13 Jun 2023 05:31:22 GMT  
		Size: 111.4 MB (111351945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
