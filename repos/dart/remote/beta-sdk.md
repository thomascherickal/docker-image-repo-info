## `dart:beta-sdk`

```console
$ docker pull dart@sha256:f3df2763083980b921e7aff12e69b986bf49795a44320cd66e310bd018ae2536
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:347ce830d2c68ecb8f0089f0945f12333e5867c6063e90ec402682584ece7c66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275791721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd043bab6007485b6961f25f971fa16264db8ba4f611dd1d44c21abab11e2f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:13:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:13:38 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:13:38 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:13:38 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:13:38 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:14:07 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=afd52527908e2184301873ef2252e13ed3d9938d47acff26297b45376d165e51;             SDK_ARCH="x64";;         armhf)             DART_SHA256=b41216eb894471a3fa6646319f5def4fe7c5115d8be9b664754a7d02a9130c6b;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3045035160b0af67111cd28aef5d8cbd50d264deb279d23e77767a0a2137a236;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1caab2cc88d2bfef34fc56a9f094f5065d8b9ac996e4afeaa664e4484f75f65`  
		Last Modified: Wed, 20 Apr 2022 07:14:35 GMT  
		Size: 45.1 MB (45072693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c033219b7813c4cd899bc0748dcfac42c25d78a696fd5da94eeda7ef1dd8562`  
		Last Modified: Wed, 20 Apr 2022 07:14:28 GMT  
		Size: 2.1 MB (2139552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca96c17ef048ced7388deecf022a8f76f118e7aa0c24386de49d423903893ac`  
		Last Modified: Wed, 20 Apr 2022 07:15:53 GMT  
		Size: 197.2 MB (197200497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:6727a046920472dec2502644706ce973a6b2d5cbd716a554b6c6ce85f1750bc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.1 MB (184077668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d877f0e105911d51948b657ed7beed93c71debe85a4ac1018a4ba1364368f3d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:50:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:50:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 20:50:43 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 20:50:43 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 20:50:44 GMT
WORKDIR /root
# Wed, 20 Apr 2022 20:51:43 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=afd52527908e2184301873ef2252e13ed3d9938d47acff26297b45376d165e51;             SDK_ARCH="x64";;         armhf)             DART_SHA256=b41216eb894471a3fa6646319f5def4fe7c5115d8be9b664754a7d02a9130c6b;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3045035160b0af67111cd28aef5d8cbd50d264deb279d23e77767a0a2137a236;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5128dd097d08ca6e030832d392aff57df592d503fd9f8927c4831056bd15eb9`  
		Last Modified: Wed, 20 Apr 2022 20:53:20 GMT  
		Size: 41.0 MB (40966671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d75d0f36fdc93d65e1d2abd95d63816ec15230b3c1702213f2f90899d89533`  
		Last Modified: Wed, 20 Apr 2022 20:52:57 GMT  
		Size: 1.3 MB (1288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6466b6bc3bb1fa9bf2e14ca0daf4ec7464ee4581ee40c18afc54d3b4ea4f9199`  
		Last Modified: Wed, 20 Apr 2022 20:56:13 GMT  
		Size: 115.2 MB (115247158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:14bbe04eb7832293df6a4d603e19227bf34b523797ffb570bf48c82d0e2af025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.1 MB (193144152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cdb12a557a5350c9540896f9ced952cca2b382b07e7664c20ec43a3010b1b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:06:55 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:06:56 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 20 Apr 2022 07:06:57 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 20 Apr 2022 07:06:58 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 07:06:59 GMT
WORKDIR /root
# Wed, 20 Apr 2022 07:07:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=afd52527908e2184301873ef2252e13ed3d9938d47acff26297b45376d165e51;             SDK_ARCH="x64";;         armhf)             DART_SHA256=b41216eb894471a3fa6646319f5def4fe7c5115d8be9b664754a7d02a9130c6b;             SDK_ARCH="arm";;         arm64)             DART_SHA256=3045035160b0af67111cd28aef5d8cbd50d264deb279d23e77767a0a2137a236;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.17.0-266.1.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5224c49f1d6ea5a648b1560bb384a0be9fc6ff3c7e310d18312405ade51d9e`  
		Last Modified: Wed, 20 Apr 2022 07:08:10 GMT  
		Size: 44.8 MB (44789156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be3f5b9fa7637985357830365527bb1813dbf5d63928ff1da2502af3f97c324`  
		Last Modified: Wed, 20 Apr 2022 07:08:03 GMT  
		Size: 1.6 MB (1556721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88235d328b0960e4cd8aa3a3dc378c20bb96bd28c08b5ad0acf4803a1895fcef`  
		Last Modified: Wed, 20 Apr 2022 07:09:14 GMT  
		Size: 116.7 MB (116732474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
