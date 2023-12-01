## `rust:alpine3.17`

```console
$ docker pull rust@sha256:45efe60140a6b267231dca2082c72f9437df55f9a668799b942c059a51ce6e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.17` - linux; amd64

```console
$ docker pull rust@sha256:7091c974aaf856075fc320b895e267e48ef59504512bac02b3b8767f7c483557
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.7 MB (275715322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:214964d6f8e88198f53d0fc40bf946a2abc6a7537bb4fbdbe064a982b6842b76`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:50:03 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 01 Dec 2023 07:50:03 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.74.0
# Fri, 01 Dec 2023 07:50:22 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef39ec453e72776182dce80d9f9e5759c11379a8f8e5263d99e1db99fe5534b`  
		Last Modified: Fri, 01 Dec 2023 07:51:36 GMT  
		Size: 53.1 MB (53089474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448b09e0f88863b90fbf5556130de66d210a6a2e5807d665a8270fcbcbb59d97`  
		Last Modified: Fri, 01 Dec 2023 07:51:56 GMT  
		Size: 219.2 MB (219246525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:2d3e4e0e289b2585bc41bdc0dd99bffd5cf529e6b64d2254f27a32be1de0a08c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279629164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604265ccd3db3d22b89bc75d6f519a245e43a74475af2742aad0ffdace6c6ebb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:01:18 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 16 Nov 2023 21:08:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.74.0
# Thu, 16 Nov 2023 21:08:31 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ca32672903471782a46d0fd4f81a60219ffe88c811df599489e89b42425516`  
		Last Modified: Sat, 21 Oct 2023 03:03:01 GMT  
		Size: 45.6 MB (45608852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe0d28bd9f0f0b5f5550fb2ec9bf71215c3aab0f7e8552ad107c4939df68199`  
		Last Modified: Thu, 16 Nov 2023 21:14:36 GMT  
		Size: 230.8 MB (230762022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
