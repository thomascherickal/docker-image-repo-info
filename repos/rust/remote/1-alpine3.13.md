## `rust:1-alpine3.13`

```console
$ docker pull rust@sha256:5a3094f3898d869597cccd5cd8a9dc991578d7ac1227531003396d1b85551053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.13` - linux; amd64

```console
$ docker pull rust@sha256:762d1b3252a8ac4bae7643092333f5be0923755babe65483868760a4bd431dd6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (247978003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa1051427579c90d9bec8ce89efa4f5a383e45fd7e8fb2a2c5af2c3a3996b2d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 06:56:05 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Feb 2021 06:56:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Thu, 18 Feb 2021 06:56:25 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e28739f2483627c62c687564cedd1a93a5ecab4332a45dcc260fd5e3398face`  
		Last Modified: Thu, 18 Feb 2021 06:57:11 GMT  
		Size: 42.2 MB (42173663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abc17832dcebc3c3e2db4c25d77e10bda4b3628e2385bb55eab4f9a294e986`  
		Last Modified: Thu, 18 Feb 2021 06:57:39 GMT  
		Size: 203.0 MB (202992683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:b55902ea5f0dbede9207cdfe8c8121cee9183f29e7dff788d8a4643c6511e4f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223902582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1bf15f368ddec10a307bdc833227660114602f8d43090afb339b4b71e69897a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:25:27 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Feb 2021 01:25:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Thu, 18 Feb 2021 01:25:56 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee793ae8b7999b4d1b06d5afd26bdc775d4dfbbbe2dd9df4c518cbeb486e896f`  
		Last Modified: Thu, 18 Feb 2021 01:26:54 GMT  
		Size: 35.9 MB (35928154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81c6a1143abd7a94fc52b6e71936054a8a8afa5f52aae4d62e5c2899bd7a04b`  
		Last Modified: Thu, 18 Feb 2021 01:27:34 GMT  
		Size: 185.3 MB (185262856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
