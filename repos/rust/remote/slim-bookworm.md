## `rust:slim-bookworm`

```console
$ docker pull rust@sha256:26e2eadb404be7ddf123b821a9af32865894c21ad8066ab70722c1c7d04d64f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bookworm` - linux; amd64

```console
$ docker pull rust@sha256:d9200b513cf30945c9b2fd1a9515c5a51d2ad9986f4f8c73369c72c3f92d333a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.2 MB (277189590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8139dbabba41f6afa2f2fbc52ed6c8d361811961d196f46400d6957ef91d55c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:03 GMT
ADD file:54d8c2ef68f89eb97aafa6f54145d4a26b2a6c9dd8b7a924515e5c5194ea5413 in / 
# Thu, 23 Mar 2023 01:30:04 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 01:30:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Fri, 24 Mar 2023 01:31:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:96af4d596c1b029a6658834de0689aadff93ec5d1dc062654678440b2cfda787`  
		Last Modified: Thu, 23 Mar 2023 01:33:45 GMT  
		Size: 29.1 MB (29073181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8cc5afc8f24313fae03bb97dafd1aeb4da66cec11fd4fa9bfddbbade899907`  
		Last Modified: Fri, 24 Mar 2023 01:36:16 GMT  
		Size: 248.1 MB (248116409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm variant v7

```console
$ docker pull rust@sha256:51c8cc6d9270beaf287804618c5bd956aa43ae54c4c828d6ceea9a854087c490
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284357378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c728fba20392800cf05cca42197f86a90b2ded56f70d4e70481f3834b273c35d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:11 GMT
ADD file:8292555b52d2bb56959d4eb73174e182ce8ae231ddce0385e0177b9f325f774e in / 
# Thu, 23 Mar 2023 01:13:12 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 22:35:26 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Thu, 23 Mar 2023 22:36:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:df7162aa8cb926599b6249fd43b78b8dbf70d2400e56898782927be1a883817f`  
		Last Modified: Thu, 23 Mar 2023 01:32:46 GMT  
		Size: 25.7 MB (25681928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70716c454d27fd46d843c199374ba54307663e9f80f120ad7541b920ace34f8`  
		Last Modified: Thu, 23 Mar 2023 22:41:02 GMT  
		Size: 258.7 MB (258675450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:4375b0168b767ce3e4ced299dbddc43a4e53cca4c59060665e30a34669c0949f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338161242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4affa004a52db313655b041fd083b488245ecd6aa89dd1986643a27660e4c8b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:55 GMT
ADD file:b3c7cfb1fd031012c20cd6ee37e3c98495a4c4af45480d83b8b16d9a7ba83c70 in / 
# Thu, 23 Mar 2023 00:44:56 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 22:35:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Thu, 23 Mar 2023 22:36:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:015f7b32198b1c57333fa9e151a0b54ccfe05dfef57e98b87c27d426f134db80`  
		Last Modified: Thu, 23 Mar 2023 00:47:30 GMT  
		Size: 29.1 MB (29117766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7cb7b36bb2b685a119a64a871e0c3b5da90ef0598c9283eec2c7980b68f164`  
		Last Modified: Thu, 23 Mar 2023 22:41:58 GMT  
		Size: 309.0 MB (309043476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; 386

```console
$ docker pull rust@sha256:5d646b43b89aeda7f007ba7fbbf21572ec0de9a4d1650af5c1389f5a73ea9cca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290123177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8321fba80cf0b36e35c11546a6a42b07ef8ff752459f419540b66c3adbfc84`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:38:56 GMT
ADD file:6c9e0efe1662b8e2fdc9cf2609c3258578c9f7ff6383768c1d15bbeaaf0a2241 in / 
# Thu, 23 Mar 2023 00:38:56 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 04:54:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.68.1
# Fri, 24 Mar 2023 04:55:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='bb31eaf643926b2ee9f4d8d6fc0e2835e03c0a60f34d324048aa194f0b29a71c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6626b90205d7fe7058754c8e993b7efd91dedc6833a11a225b296b7c2941194f' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='4ccaa7de6b8be1569f6b764acc28e84f5eca342f5162cd5c810891bff7ed7f74' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='34392b53a25c56435b411d3e575b63aab962034dd1409ba405e708610c829607' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.2/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4c769a1c6b01d4570b6cf392bd1d972d4b964ad818a2f349fddd8089db9b735c`  
		Last Modified: Thu, 23 Mar 2023 00:42:26 GMT  
		Size: 30.1 MB (30104962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ed282937ae8146f0e3b7db4c93b372def65ef08c91ba689e0054e372cbef0d`  
		Last Modified: Fri, 24 Mar 2023 05:01:26 GMT  
		Size: 260.0 MB (260018215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
