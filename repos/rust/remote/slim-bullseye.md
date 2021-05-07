## `rust:slim-bullseye`

```console
$ docker pull rust@sha256:0019a2286235aea52d97f74250f41aa57c1e457a6bad7f7d34a0fa967d6afe5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:e624fd294871a36515da4392ae34f09537ca901341e7ddf1cc88ebc3321f798e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227334905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2a82a32cd0021b1b11d8799b867eb39ee04cb261101276ab474476825c3ba7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:19:58 GMT
ADD file:355194a9b58fc933fe444d7866cc4a39713a870a65402d65440a2dc357735259 in / 
# Sat, 10 Apr 2021 01:19:58 GMT
CMD ["bash"]
# Fri, 07 May 2021 01:59:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.52.0
# Fri, 07 May 2021 01:59:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='fb3a7425e3f10d51f0480ac3cdb3e725977955b2ba21c9bdac35309563b115e8' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f263e170da938888601a8e0bc822f8b40664ab067b390cf6c4fdb1d7c2d844e7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='de1dddd8213644cba48803118c7c16387838b4d53b901059e01729387679dd2a' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='66c03055119cecdfc20828c95429212ae5051372513f148342758bb5d0130997' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:59d01ccdd87174a9ae0eb936ee6947e974e2b30eaa69a472f92ce378f07176ef`  
		Last Modified: Sat, 10 Apr 2021 01:24:28 GMT  
		Size: 31.3 MB (31347743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d84c9b7d2599a408f9a16c1ae6966ba9fee0e59cc34dc46a20bdec1757fb15d`  
		Last Modified: Fri, 07 May 2021 02:04:04 GMT  
		Size: 196.0 MB (195987162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:2b348bceb61f37121e388dea79ce0a11c706fe21b1cb149116f829ad466097d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.7 MB (247690213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518f2c768d60879147971ded740e7e6fd851213673ac78b2a54f80b5be69faf4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:58:54 GMT
ADD file:49314be3b948dd917c99b41c532d83ae6749173379fe4a80d8e4ad55b2d89c6e in / 
# Sat, 10 Apr 2021 00:58:56 GMT
CMD ["bash"]
# Fri, 07 May 2021 02:37:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.52.0
# Fri, 07 May 2021 02:38:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='fb3a7425e3f10d51f0480ac3cdb3e725977955b2ba21c9bdac35309563b115e8' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f263e170da938888601a8e0bc822f8b40664ab067b390cf6c4fdb1d7c2d844e7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='de1dddd8213644cba48803118c7c16387838b4d53b901059e01729387679dd2a' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='66c03055119cecdfc20828c95429212ae5051372513f148342758bb5d0130997' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:535f9c9bd2387fe5771446f92b5683c8f2986c9ad78ddfd34210e0dbc8457937`  
		Last Modified: Sat, 10 Apr 2021 01:07:01 GMT  
		Size: 26.6 MB (26552221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fce69e3f93242cfc6a78f40e1c5970a5d056eeead3c5a2b992d39b1ce76b62`  
		Last Modified: Fri, 07 May 2021 02:43:47 GMT  
		Size: 221.1 MB (221137992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:5e5e9504ec47a51f8a37511a5a021b71525e591b089466499f2afa112a7a862f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.4 MB (278422750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be96d96fee7a68126e2d1f0e5479159da156795577c4dc4963f2b682d6cb762d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:42 GMT
ADD file:52386542816793aa41ac6565bc866fb10b7784d3bab5dfbc3bb55624d9de634f in / 
# Sat, 10 Apr 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 07 May 2021 01:23:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.52.0
# Fri, 07 May 2021 01:25:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='fb3a7425e3f10d51f0480ac3cdb3e725977955b2ba21c9bdac35309563b115e8' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f263e170da938888601a8e0bc822f8b40664ab067b390cf6c4fdb1d7c2d844e7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='de1dddd8213644cba48803118c7c16387838b4d53b901059e01729387679dd2a' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='66c03055119cecdfc20828c95429212ae5051372513f148342758bb5d0130997' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:a4f78f5edc1a83a6ef24abc7ff6722c452292a1f4ea954365aecbab9c7fc1861`  
		Last Modified: Sat, 10 Apr 2021 00:47:11 GMT  
		Size: 30.0 MB (30037067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e5f9caba4e660d259cbe88680295a5a19c17f52d42a65abbbe9750b806436`  
		Last Modified: Fri, 07 May 2021 01:31:28 GMT  
		Size: 248.4 MB (248385683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:3885229f05a54933b52ba2495e8f3209b97b8196bc2c9eb3e63e73eea7a58926
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.0 MB (268007140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e426490209e22d6d3d767764cee30984390cae95cb490312dae015e821dcbb6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:13 GMT
ADD file:d201ac3b33d7c359a0ba889539c9fbce9647142726109af896aa8b053cec35e5 in / 
# Sat, 10 Apr 2021 00:39:14 GMT
CMD ["bash"]
# Fri, 07 May 2021 01:49:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.52.0
# Fri, 07 May 2021 01:50:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='fb3a7425e3f10d51f0480ac3cdb3e725977955b2ba21c9bdac35309563b115e8' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='f263e170da938888601a8e0bc822f8b40664ab067b390cf6c4fdb1d7c2d844e7' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='de1dddd8213644cba48803118c7c16387838b4d53b901059e01729387679dd2a' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='66c03055119cecdfc20828c95429212ae5051372513f148342758bb5d0130997' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:baff5217fbd64e583e92ee39435c69cc22ba0b3b14dffcb0f60f4e9b82bf6c36`  
		Last Modified: Sat, 10 Apr 2021 00:45:04 GMT  
		Size: 32.4 MB (32365969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860dd3f8d74febbbd7e35341f9d35824e6ac84c33f93020a741e79f324f464b7`  
		Last Modified: Fri, 07 May 2021 01:55:39 GMT  
		Size: 235.6 MB (235641171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
