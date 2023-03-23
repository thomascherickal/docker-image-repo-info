## `dart:latest`

```console
$ docker pull dart@sha256:a5bf4aa6a6b81ce57c82f002b76f71f43ec29b589505bfb9b8054b4b97a5b43f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:de9bcd1f2d911c98f57c502c68dd9410972464b646623da74362cecff5b8b11f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300589270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1224e9d338b32ccc9fc2002cf876d34da7f28d7f2fc12b698211f933403de97`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:35:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:35:58 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Thu, 23 Mar 2023 06:35:59 GMT
ENV DART_SDK=/usr/lib/dart
# Thu, 23 Mar 2023 06:35:59 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:35:59 GMT
WORKDIR /root
# Thu, 23 Mar 2023 06:36:14 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f8591944512834ba19b4d8383d270d7f56fef03c56ba53d4e35c23db80ea8a33;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a87833fbfed26ef810cb135c47eb7b5bc24c906b55abb4a2e183fea2d3ce1b51;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c81303feea24228148bd4ec14c65bb9c341cba3596e3d68e8a874a9df947f928;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413fb299252e01cce0ab0f8ca7a4b07c54b168de5f22d30f344ef1e4e9e56315`  
		Last Modified: Thu, 23 Mar 2023 06:36:56 GMT  
		Size: 45.1 MB (45102666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5b7c0a9a8675f9fddb6877fa45f4558ec79c4e1f4746a9ee6d9e5d83b4c40`  
		Last Modified: Thu, 23 Mar 2023 06:36:50 GMT  
		Size: 2.2 MB (2162022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cc2ededdf85d1e35427a75b3e96b300624432ebd7cf76af3d179fc11e6a088`  
		Last Modified: Thu, 23 Mar 2023 06:37:20 GMT  
		Size: 221.9 MB (221913177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:609d4d52728feaa977573d122f508bbffca2a30de0f388cf77e98807a6ce180a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3264d5e28e14c2271c861e03d2fe9cf0cacef6b81d162ddff59b9246f4140c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:25:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:25:08 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 01 Mar 2023 02:25:08 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 01 Mar 2023 02:25:08 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 02:25:08 GMT
WORKDIR /root
# Wed, 08 Mar 2023 19:57:40 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f8591944512834ba19b4d8383d270d7f56fef03c56ba53d4e35c23db80ea8a33;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a87833fbfed26ef810cb135c47eb7b5bc24c906b55abb4a2e183fea2d3ce1b51;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c81303feea24228148bd4ec14c65bb9c341cba3596e3d68e8a874a9df947f928;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a2a2202be4ce8d1e3c64eeb5cd1a880b653007a431bebfcb9aa6b27ac927e`  
		Last Modified: Wed, 01 Mar 2023 02:26:29 GMT  
		Size: 41.0 MB (40988626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2c1c5227941118e0a1f640f63b2b993bb7b3e42883849a783c7f7cd6d4487`  
		Last Modified: Wed, 01 Mar 2023 02:26:22 GMT  
		Size: 1.3 MB (1288541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d0b0c5c959e308c5938a53ab55713c9532f9ba8543358c36ac069b3a38c693`  
		Last Modified: Wed, 08 Mar 2023 19:58:56 GMT  
		Size: 127.9 MB (127903417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:86a4212ab6616b992fd3cdd79009f27d4c75ec304d4ca91814196d2f82d5f981
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205987120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79b78c4830bef627d3407546efbc45aa4399732548715a20c239f206bd60439`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:03:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:03:50 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 01 Mar 2023 13:03:50 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 01 Mar 2023 13:03:50 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 13:03:50 GMT
WORKDIR /root
# Wed, 08 Mar 2023 19:39:29 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=f8591944512834ba19b4d8383d270d7f56fef03c56ba53d4e35c23db80ea8a33;             SDK_ARCH="x64";;         armhf)             DART_SHA256=a87833fbfed26ef810cb135c47eb7b5bc24c906b55abb4a2e183fea2d3ce1b51;             SDK_ARCH="arm";;         arm64)             DART_SHA256=c81303feea24228148bd4ec14c65bb9c341cba3596e3d68e8a874a9df947f928;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.19.4/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad58cbb76aa261586e238ac663c806e6da6fda3059b45385c8c3938a59387`  
		Last Modified: Wed, 01 Mar 2023 13:04:43 GMT  
		Size: 45.0 MB (45011137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f122052879f43039ebbbbe28f2f87037e49d388f36058bf9b4f1e579229b1a`  
		Last Modified: Wed, 01 Mar 2023 13:04:38 GMT  
		Size: 1.6 MB (1562174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4156da6bde6632660a8a6c95c0df6b9d0c6cd616954975826366695fe8642d23`  
		Last Modified: Wed, 08 Mar 2023 19:40:08 GMT  
		Size: 129.4 MB (129350995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
