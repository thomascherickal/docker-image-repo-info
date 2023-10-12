## `dart:beta`

```console
$ docker pull dart@sha256:81eff69e362531665e108a78564e3393bc6213ba60622f3d5ea628d72d532b09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:9dd03ab192e57898cda87fbc29372681077a6a8a771aeb4aeeb180b7bc68e03b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308566596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ac7ff757fb4edfbf534b18372c78adfcfbbc5ce8207a58f724c90fe5e8e7e41`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:35:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:35:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 22:35:04 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 22:35:04 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:35:04 GMT
WORKDIR /root
# Wed, 11 Oct 2023 22:35:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d10d4aa2daf2afc43397ea4c4106a9965c2930bed022ee4d9e8f195cb856af41;             SDK_ARCH="x64";;         armhf)             DART_SHA256=070729edebd45adca5f7c023df7b887787452bdc4417682fbbf366712bd7d338;             SDK_ARCH="arm";;         arm64)             DART_SHA256=305ca5698e0399bc5cb96c394d158ceb83be59e9dc83b761c2b4dac2769e2af0;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c0bb5fb66e490a1f05f4cd349d80465ae33ca359c4fb68dd1c74e658176ca`  
		Last Modified: Wed, 11 Oct 2023 22:36:10 GMT  
		Size: 54.6 MB (54639187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb3d09a7f21147b48a35dce85aae05f8811cd31156fc58a275aec435712e16`  
		Last Modified: Wed, 11 Oct 2023 22:36:02 GMT  
		Size: 1.8 MB (1800644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b75ba1ec6b07bd2e5c3233e593880ed3b590b2d2a63cca6f6ce3b43aa075aec`  
		Last Modified: Wed, 11 Oct 2023 22:37:26 GMT  
		Size: 223.0 MB (222976891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:c6cffacd175ecb80015fedfdd7bf3bc6e1bea0c8ea49a186139a16614bf5f1b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203521137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0b1af82226a721b8c03657e35195dbf25ab7536b284eef034faad5a5c39e6f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:21:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:22 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 11 Oct 2023 18:21:22 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 11 Oct 2023 18:21:22 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 18:21:23 GMT
WORKDIR /root
# Wed, 11 Oct 2023 18:21:57 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d10d4aa2daf2afc43397ea4c4106a9965c2930bed022ee4d9e8f195cb856af41;             SDK_ARCH="x64";;         armhf)             DART_SHA256=070729edebd45adca5f7c023df7b887787452bdc4417682fbbf366712bd7d338;             SDK_ARCH="arm";;         arm64)             DART_SHA256=305ca5698e0399bc5cb96c394d158ceb83be59e9dc83b761c2b4dac2769e2af0;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df7c1334c06ce61f50070f4f0982f1670c0f9ce6d68f66c53d97df089773bd`  
		Last Modified: Wed, 11 Oct 2023 18:22:22 GMT  
		Size: 49.2 MB (49197359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43deeabde0db6379fcbf973ad8d851910371d49793774b9e405fb517bcb5efe0`  
		Last Modified: Wed, 11 Oct 2023 18:22:15 GMT  
		Size: 1.2 MB (1227230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aca3211574cba3a679289c44f735c5b1b4ba07df25dab2e4e8c4e34bee6ba9`  
		Last Modified: Wed, 11 Oct 2023 18:23:20 GMT  
		Size: 128.3 MB (128347623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:e0a0eed705fe560ada11837bffd84779f3ddcb91b93b21ec5d6e95381674a0f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.7 MB (213721852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57e3205b0d6bf569b22eaaa3c7be5c232e4f17518c53209d12627eb2980e2cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:17:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:17:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 12 Oct 2023 10:17:40 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 12 Oct 2023 10:17:40 GMT
ENV PATH=/usr/lib/dart/bin:/root/.pub-cache/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:17:40 GMT
WORKDIR /root
# Thu, 12 Oct 2023 10:18:04 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=d10d4aa2daf2afc43397ea4c4106a9965c2930bed022ee4d9e8f195cb856af41;             SDK_ARCH="x64";;         armhf)             DART_SHA256=070729edebd45adca5f7c023df7b887787452bdc4417682fbbf366712bd7d338;             SDK_ARCH="arm";;         arm64)             DART_SHA256=305ca5698e0399bc5cb96c394d158ceb83be59e9dc83b761c2b4dac2769e2af0;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/3.2.0-210.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7edca539e4b60c13376b1f5419e9fa3efb2541d698345e3ee79bc0dcb6e374`  
		Last Modified: Thu, 12 Oct 2023 10:18:27 GMT  
		Size: 54.3 MB (54318879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59a1c0a25c7682a3b440ea832050e935d14e0586689fdae3f67be067e1ffe86`  
		Last Modified: Thu, 12 Oct 2023 10:18:21 GMT  
		Size: 1.5 MB (1493545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11adea75e25d766111e2750ba526f5a715c5d7015bdf264555ed29564fdac5ce`  
		Last Modified: Thu, 12 Oct 2023 10:19:10 GMT  
		Size: 128.7 MB (128730144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
