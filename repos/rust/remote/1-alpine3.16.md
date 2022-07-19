## `rust:1-alpine3.16`

```console
$ docker pull rust@sha256:26d3406ed01076d53cf13b95397f2695fbb965e42aa685bca8045dcf11055904
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.16` - linux; amd64

```console
$ docker pull rust@sha256:0ebddf3a3a92320ff15b6cd3c5603ad109d71dd241ebfbda5a3c79acd91fa7ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244164257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a83e7ec7491adfa83edde65f415fd133d3a47fd6be9b2b1843b46d3a188c4da`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:47:32 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Tue, 19 Jul 2022 17:04:00 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.62.1
# Tue, 19 Jul 2022 17:04:20 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a520168a06cb7152566b84f67136c71b6ead2361120ff23f5215602e80ac64a`  
		Last Modified: Mon, 18 Jul 2022 23:48:52 GMT  
		Size: 41.4 MB (41419552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a77380093fe4a2872c0b2507c0bfe8630be5b6e615c7bde564600ddc893a1a2`  
		Last Modified: Tue, 19 Jul 2022 17:09:13 GMT  
		Size: 199.9 MB (199945899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:3ec9c7667d9d83ab5745fa44d3298eef0e3ddffbf0fb4cf917a81b75a5fee8f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244315724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34ba6be81569c3b21573c71cb19489b19809e79d5744611dc982b4cff587c1e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:08:15 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Tue, 19 Jul 2022 17:15:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.62.1
# Tue, 19 Jul 2022 17:15:47 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eed4d3d2736c6a52d47bbb88593b623d6475eea1bd6b5c9af3aac9e546514ee`  
		Last Modified: Tue, 19 Jul 2022 03:10:11 GMT  
		Size: 37.2 MB (37185897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e7a664aa4931b2f4ade470ab202cf3e490b58f7586e69b8fd5e7a53012bb20`  
		Last Modified: Tue, 19 Jul 2022 17:22:15 GMT  
		Size: 204.4 MB (204435107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
