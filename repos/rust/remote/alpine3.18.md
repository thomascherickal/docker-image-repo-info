## `rust:alpine3.18`

```console
$ docker pull rust@sha256:8f88a945dd8af49c6ce4f6d92666588c382bfa57c9ec50621f03f006ac389d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.18` - linux; amd64

```console
$ docker pull rust@sha256:5d4632e7896c683a7a0f514bd0a3917543fb7e4ddfff514195d61f4cad422a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.2 MB (274177442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf13d7e7dda336ee3d87ee8d89b6ea5b475bd042292eca0598b08a9f047bc091`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:50:32 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 01 Dec 2023 07:50:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.74.0
# Fri, 01 Dec 2023 07:50:49 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475ae4a9ddfa93b5af31dec0c2238fb02d679c1e4471b62bb52414567fe43e2c`  
		Last Modified: Fri, 01 Dec 2023 07:52:17 GMT  
		Size: 51.5 MB (51528440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dee6606cefedc201138c70f9b30a61ec957191943973e080dd0f68700a7c5b`  
		Last Modified: Fri, 01 Dec 2023 07:52:39 GMT  
		Size: 219.2 MB (219246580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:e8fb372d936387cd2b804cad31d6bc6616936c6b6ff093b031e29f3a2217a6e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280160645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c455cc0b0272868c1ba7f0d90f14d17aee88f05d8496802835e3a58081aaaa9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:01:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 16 Nov 2023 21:08:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.74.0
# Thu, 16 Nov 2023 21:08:53 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10083f95cebc6d88b9b7dec1267400daef705ad0f2d9e19546e44ff81f96d0f7`  
		Last Modified: Sat, 21 Oct 2023 03:03:36 GMT  
		Size: 46.1 MB (46066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e8e0bff18e527749ea16175466d8583c76c1b538decdb2a38c97da5785cf65`  
		Last Modified: Thu, 16 Nov 2023 21:15:12 GMT  
		Size: 230.8 MB (230762280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
