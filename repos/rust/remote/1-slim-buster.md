## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:56579febe02b524a234488cfb7d318547240fc9cf3efd49f4cad3408c6c26b3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:a45521aed6694a66c6c8c9df0ad67836c0f82e50379e1c827529a766d971dc4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259516021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1e9e4191b90917dc085917e0e4fc9ac9a4fdf797564f3e4ecb33366fcb7c7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Thu, 13 Jul 2023 21:53:15 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.71.0
# Thu, 13 Jul 2023 21:53:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a23030ad8db224607eccd1ccab2315e77716800efec703fd8068d67e4080f0`  
		Last Modified: Thu, 13 Jul 2023 21:58:17 GMT  
		Size: 232.4 MB (232377519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:444831565d5e6020968d00d02af12141471644d62a930aef5c5ea173159a1ee5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266171512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94f649775ed38354ee723579452c025ca25ab174c0e95a5f3c97c2f5ffebac8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 15:29:20 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 04 Jul 2023 15:29:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7092433332eda4cb31ddf30d64b3104ea60028fa61059631637149dff4191295`  
		Last Modified: Tue, 04 Jul 2023 15:34:41 GMT  
		Size: 243.4 MB (243424215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:90ac5ea240055ed36c3b612240ace9ee1a8337532eefc4a884490698300e5c83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.0 MB (309951566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c67f62ef570be472ea5bce9d86ec6bafad0a8b16b5648f2827ab83317ace0fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:47:14 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 04 Jul 2023 13:47:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70d4b51ecd2d46f89e73c6372ed9d6633f9eee841ac19c8b540bed87982a78e`  
		Last Modified: Tue, 04 Jul 2023 13:51:34 GMT  
		Size: 284.0 MB (284030111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:518b852f14c671b4684367f9dc62bc2a0c5252d323f55b8c673c990694612e86
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.7 MB (270744127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2062acf3c34fc3bfe103ddba73dd2457017a4a1861065c888c7900c5198a2fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:22 GMT
ADD file:0be890be1c2ff0966cf1b714bd814e6859e1a2cb4a491ebd6c28d551eeedd66b in / 
# Tue, 04 Jul 2023 01:39:22 GMT
CMD ["bash"]
# Wed, 05 Jul 2023 01:27:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Wed, 05 Jul 2023 01:27:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:b4637b85bb10ca071ae2bfe4ea2e6dd6ca216cecae3d9db6787e67046e0c1f70`  
		Last Modified: Tue, 04 Jul 2023 01:44:56 GMT  
		Size: 27.8 MB (27797000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80000eb655a8877493cde035b226881dcac8553243cc1556aaf4ad3dbafff5a3`  
		Last Modified: Wed, 05 Jul 2023 01:32:26 GMT  
		Size: 242.9 MB (242947127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
