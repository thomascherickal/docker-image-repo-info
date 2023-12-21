## `dart:beta`

```console
$ docker pull dart@sha256:20a61a53046b1c433f7eb0f0f809cb08b4971b643bf6d3fc75916eba7950a53a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:c42fd4285aa48eb1904278fe1e87cd0d2ae3dba8c61f1e2e74db3f853c5a1bc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309404645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b041ec241a3323db182ff7c5fef96574ffc37d423957c6aec9ea42e0f0b182f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:49:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:49:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 19 Dec 2023 04:49:50 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 19 Dec 2023 04:49:50 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 04:49:50 GMT
WORKDIR /root
# Thu, 21 Dec 2023 21:30:33 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=24fee21a8e378050b0b0611602f674059d5a93bb09a560539857e384f1b83056;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2cccf79d89105294c46881f0f7d7e1f574d6cb2d8a12de7d0a04311dcde6acb2;             SDK_ARCH="arm";;         arm64)             DART_SHA256=f86de4ab4f99a2dbdc6a0809acaae40a280fa3cbac340bbdf910cf7f0085dcbb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.3.0-174.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a05f793f09b881884ae5ad6ca2a954523e8028b980eed591fc8b48dc2960350`  
		Last Modified: Tue, 19 Dec 2023 04:50:49 GMT  
		Size: 54.6 MB (54643992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baf096ff6e9a5ca1347d22327e218f52f0313d7795e0988bddbe07b0e8b5a17`  
		Last Modified: Tue, 19 Dec 2023 04:50:42 GMT  
		Size: 1.8 MB (1800653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37e5318388b6c1b4f038988926373abcd4dedb554e56944b3901b9eab41d67`  
		Last Modified: Thu, 21 Dec 2023 21:32:16 GMT  
		Size: 223.8 MB (223834037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:08659cbc5bf1b5f3ce6f9aab7aa326f45a3724914397293025b60f22dbad4827
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202842962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c28650addaf392268ee96f68d81019cf4da9373e6f1333abea961dd04cf09a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:52:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:52:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 19 Dec 2023 07:52:29 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 19 Dec 2023 07:52:30 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 07:52:30 GMT
WORKDIR /root
# Tue, 19 Dec 2023 07:52:59 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=3b58bb6ff1ba2580858e2e9ad0a1f358246ba545bdd092a475f62e6aa1396394;             SDK_ARCH="x64";;         armhf)             DART_SHA256=c53268123dcaf9adfed22545999c626a7a2a33387406d514148847fa8191afb9;             SDK_ARCH="arm";;         arm64)             DART_SHA256=6eb38bec0f3167e7f892e2d074aa2b30bfb456b8f4b204acda453af4ca27dd1b;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.3.0-174.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5826252357d0dc1a6f3112bc82861ed1897daa44db08861e7db3b3bda8c13c`  
		Last Modified: Tue, 19 Dec 2023 07:53:22 GMT  
		Size: 49.1 MB (49146903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff35e7f3baf8c9515e067454abc3bf732480590c25a0ad070c27247c1358c92`  
		Last Modified: Tue, 19 Dec 2023 07:53:13 GMT  
		Size: 1.2 MB (1227208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98c75d537092396d8d1910bdc665b69884fd96b312dc0eb195a711fb2315891`  
		Last Modified: Tue, 19 Dec 2023 07:54:24 GMT  
		Size: 127.8 MB (127750694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:dfc97db2594271f539e7ddcacb73718804f7e3fc698d5601df5569c145f35841
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.0 MB (308005887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116624c693dcb545b3ff8d3f316630ae8f2341871b3ad254edf60e37aff033cd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:25:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:25:03 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 19 Dec 2023 07:25:03 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 19 Dec 2023 07:25:03 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 07:25:03 GMT
WORKDIR /root
# Thu, 21 Dec 2023 21:40:35 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=24fee21a8e378050b0b0611602f674059d5a93bb09a560539857e384f1b83056;             SDK_ARCH="x64";;         armhf)             DART_SHA256=2cccf79d89105294c46881f0f7d7e1f574d6cb2d8a12de7d0a04311dcde6acb2;             SDK_ARCH="arm";;         arm64)             DART_SHA256=f86de4ab4f99a2dbdc6a0809acaae40a280fa3cbac340bbdf910cf7f0085dcbb;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.3.0-174.3.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5382a32fd6fb3d0650e271153f9d2090471f18e9b0aebc4d682998e6f31c64d6`  
		Last Modified: Tue, 19 Dec 2023 07:26:01 GMT  
		Size: 54.3 MB (54311966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6782c98493ed0507fc2e0c7a8dde5c86e1b5e0590fbabde016ce6f1e62481acc`  
		Last Modified: Tue, 19 Dec 2023 07:25:56 GMT  
		Size: 1.5 MB (1493555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9332ed6ca02900bac2d8ad268418902494af4988012ab08356fe7f8b19d0cd2`  
		Last Modified: Thu, 21 Dec 2023 21:42:03 GMT  
		Size: 223.0 MB (223043097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
