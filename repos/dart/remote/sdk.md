## `dart:sdk`

```console
$ docker pull dart@sha256:1521c3d4e9e077a306e6af0857f49dd9465333cd0d140677c99a73c81582a63f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:167f3b7a768d37c813a953faf72b82c6f2ccbca1e753a960371d413088139b78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296148926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0033636b7f808df29a950bc00984ace57d845ebe46ef5a51f250c25eae9a29`
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
# Wed, 11 Oct 2023 22:35:17 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0150dff731ac017646941ebfa46ca2a7bbe5c634be0928262d524420341fc739;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0edf3fe2f5b8d212468de67b08fd1f27e5a775ef10e4e8bbef811a083cf15650;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2b2830001cd8732d356c4beee7be25c947e6cb6e8ca7b8ea748da47f6cc9d222;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:de411aff59341d6595bab5539c27772abfccd06ff52dc714d5d7fbe46570febc`  
		Last Modified: Wed, 11 Oct 2023 22:36:30 GMT  
		Size: 210.6 MB (210559221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:2f7245226858ea86fffbdbb30de8333a45a3a14e26352eff89420b0c9de62385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187100537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68c112737de71b07ef8bd0713cba469929b87fba3e4b1c87f1b802f86c0c273d`
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
# Wed, 11 Oct 2023 18:21:36 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0150dff731ac017646941ebfa46ca2a7bbe5c634be0928262d524420341fc739;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0edf3fe2f5b8d212468de67b08fd1f27e5a775ef10e4e8bbef811a083cf15650;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2b2830001cd8732d356c4beee7be25c947e6cb6e8ca7b8ea748da47f6cc9d222;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:fb99db0b9128df9e023e75b3fa7d423af28f024665d023d1a422869d8b613407`  
		Last Modified: Wed, 11 Oct 2023 18:22:33 GMT  
		Size: 111.9 MB (111927023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:9f586b8fe98e68fb7916baf90099df7d632ef0753ecbee93367d89c8f0871fff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (198039293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43b6cb6950c4acb3557035fe34777631f22cfae4f07584547202fcd475f8d094`
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
# Thu, 12 Oct 2023 10:17:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=0150dff731ac017646941ebfa46ca2a7bbe5c634be0928262d524420341fc739;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0edf3fe2f5b8d212468de67b08fd1f27e5a775ef10e4e8bbef811a083cf15650;             SDK_ARCH="arm";;         arm64)             DART_SHA256=2b2830001cd8732d356c4beee7be25c947e6cb6e8ca7b8ea748da47f6cc9d222;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/3.1.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
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
	-	`sha256:d3435b5672a034023a57b02ce94e9108ab51890fc6d5d996115690a9a9f127a1`  
		Last Modified: Thu, 12 Oct 2023 10:18:33 GMT  
		Size: 113.0 MB (113047585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
