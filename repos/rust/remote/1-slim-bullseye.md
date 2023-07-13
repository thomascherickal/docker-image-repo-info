## `rust:1-slim-bullseye`

```console
$ docker pull rust@sha256:dd7affad28b68b812de4732971c1830b7b365151179c996e8b4072faea9665ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:1d0802e07bc680c643780f1284a68295173eff5f09765ccfd9eb95b215af3768
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278530062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60533f965e98e3b67e52db86d19cd05953d581d7cde3331268922f6e753488a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Thu, 13 Jul 2023 21:54:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.71.0
# Thu, 13 Jul 2023 21:54:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c147904529f7d645120ce1b1a4ced793feda296d67bf2ac93e6d83d4d611d44b`  
		Last Modified: Thu, 13 Jul 2023 21:59:45 GMT  
		Size: 247.1 MB (247112674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:1c516afcf9601e53d27492cb10e095a0662f51a1b1b5e0a08597f9cb5ffedd0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.4 MB (279366323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:202f5ef2738d0a0e21e643a9fea1f2000807c2921a85fb1820e2ac600ee29359`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 15:30:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 04 Jul 2023 15:31:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82f532fe72a8f6dd2e891eaf8f8901289f5de6d98203eaf0c1196213fcceadf`  
		Last Modified: Tue, 04 Jul 2023 15:36:18 GMT  
		Size: 252.8 MB (252787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1de20372759e9341c5b6e8cc7b18239e91947cf5ba9ddc20c0e5903b2b9fde24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329582279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81cd3a2c44601748f021b07a8b13283f2b84dbe7cf4f5b0ca2241e82fbcf6dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:48:11 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Tue, 04 Jul 2023 13:48:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c5238c2e2ef958e8d223e0cdd5b972609d6012849564065ee11d29f5ad26ec`  
		Last Modified: Tue, 04 Jul 2023 13:53:02 GMT  
		Size: 299.5 MB (299519322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:3f96f47f88bb369560fecace0c7d23d909a2f2f1911bd59c23746f783728377a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286091256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7bf81e97c69ad5f9e67b9a8be9d7625e457be8a8797f4c9b9da6973df5eba8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Wed, 05 Jul 2023 01:28:35 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Wed, 05 Jul 2023 01:29:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f21c44b01678c645d8fbba1e55e4180a01ac5af2d38bcbd14aa665e0d96ed69a' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e7b0f47557c1afcd86939b118cbcf7fb95a5d1d917bdd355157b63ca00fc4333' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7116d40d4beb20e513026a1a54054fe6a12f5d81a1fbe96b013b5a93f8d3d83`  
		Last Modified: Wed, 05 Jul 2023 01:34:22 GMT  
		Size: 253.7 MB (253693760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
