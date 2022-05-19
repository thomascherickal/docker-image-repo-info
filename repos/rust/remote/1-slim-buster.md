## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:8345ef78f92d4b7b3f5542107396f71d42f07a9aa30a2f020828f6d693db6712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:ecf4984a4cbd456d3670449efe63c665bbf850b821c4d3a30a7dee7896d9f1cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd1e35201514da9bdc71adeb5f0ad381ce84089c40a6419d02f3a73b6845e96`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910c9723b9c8224fdc9165793746a7bdef632a394043bf09d8c357918d0d8eeb`  
		Last Modified: Wed, 11 May 2022 16:20:14 GMT  
		Size: 193.5 MB (193486525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:5787cef45a9f13e1dea2638ba8ec7d928a7d6c3e6769eef73355011f9d99f327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240262048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979601ce35358bda70bbec9cfa78b0566870036b24dc3a066b2f5e10cbae68f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:59:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:00:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445544703dfa3d6936573907d147f14265cf553e666c39769991139c3c5216f`  
		Last Modified: Thu, 19 May 2022 18:09:17 GMT  
		Size: 217.5 MB (217514184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:541f0b63df779aee4eb28f4f2ef5ec9e3b7251be6011cd39f497c8e6472019d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269122908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92aa5b1b5884c8281bde8930fdbac8d2df5495182807435346629bb2a263e5dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:57:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0503ec1485723fc8953ef8fca5ff5794d54c7f48e60e240180a9a96de34727c7`  
		Last Modified: Thu, 19 May 2022 18:02:19 GMT  
		Size: 243.2 MB (243213894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:03dd42304f522301e06612497c9c34cea732f64d94196fc16f7e18be55696cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248236964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a49488bafeb991a838b0f60a1097c2daeb50ef3baf7d3a536b33b99274c502e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:45:03 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:45:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dac1eed3e092c2db915499da260dbc53370448565b8d7dd1a904bc0f736d7a`  
		Last Modified: Wed, 11 May 2022 15:48:47 GMT  
		Size: 220.4 MB (220437815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
