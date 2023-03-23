## `rust:alpine`

```console
$ docker pull rust@sha256:5dc618f722f92ca5f0b25e72b4b9466b46dbe147c4d5404f6f7ef1735c23eb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:d119a621ae12f84ec0c5fed77c24795120ed1c7874b2428b5a6ccc0f294dbe18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.9 MB (275914568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7729207f6518a4f128619d5540bedf4a950442751e853e136607fcf44a98411`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:51:47 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 09 Mar 2023 22:23:39 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.0
# Thu, 09 Mar 2023 22:23:59 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='241a99ff02accd2e8e0ef3a46aaa59f8d6934b1bb6e4fba158e1806ae028eb25' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a2691ced61ef616ca196bab4b6ba7b0fc5a092923955106a0c8e0afa31dbce4' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2193e8b510409480dcd3850d21ab99bf9eb42edb9582ccfd801f22a8f8b637`  
		Last Modified: Sat, 11 Feb 2023 13:53:57 GMT  
		Size: 53.1 MB (53091110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39feef52d17fa34fa51fcb31278b2d6f18d4b6c5670e8140cabcf2d4a55c51f5`  
		Last Modified: Thu, 09 Mar 2023 22:30:14 GMT  
		Size: 219.4 MB (219449012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0aadc57f60d9bad8615e3589beba88b7db2c80e23d7ce5cf7023de9d5e0fbca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.4 MB (274351417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5684f40b579cebeb3891a320d28f85a84f85a016bb253a07ad37dc19bd217b5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:38:47 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 23 Mar 2023 22:37:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Thu, 23 Mar 2023 22:37:24 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='241a99ff02accd2e8e0ef3a46aaa59f8d6934b1bb6e4fba158e1806ae028eb25' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a2691ced61ef616ca196bab4b6ba7b0fc5a092923955106a0c8e0afa31dbce4' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d773525ffbdb6405cf3883a5974f4c9e2689007bba56c62d59d3960d59845900`  
		Last Modified: Sat, 11 Feb 2023 05:40:53 GMT  
		Size: 45.6 MB (45611225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d9bbb1c458daf3b5278fcc92c1f8db26b75d542f8106a56b6bee9d12033ab3`  
		Last Modified: Thu, 23 Mar 2023 22:43:08 GMT  
		Size: 225.5 MB (225478233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
