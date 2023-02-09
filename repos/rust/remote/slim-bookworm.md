## `rust:slim-bookworm`

```console
$ docker pull rust@sha256:ba21d7dd980519c6909883cc97e1b69a3568b5fed6a442d5b8ca980179fa571e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bookworm` - linux; amd64

```console
$ docker pull rust@sha256:87d10e7dcc35dc5397140235b7e3aa69f307321978035dd08d4e791f28325d30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.1 MB (275099623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d1b2679d94c69eccdab9afeaa4de08bd060888ac34c03f89db8e4984a89187`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:51 GMT
ADD file:337bbae18d54468a66c653b9220ae08bec042350edd304756a97b3e60267ad76 in / 
# Thu, 09 Feb 2023 03:19:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:08:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Thu, 09 Feb 2023 07:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:7bc891379e23129e848190304442ae0e2cb2ceff0a43560520cbef46c3e03a80`  
		Last Modified: Thu, 09 Feb 2023 03:24:32 GMT  
		Size: 29.0 MB (29020258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e95fa11cd2dfe8768590e4870f16d37813fefec70cde1c380b798d9a63cdc52`  
		Last Modified: Thu, 09 Feb 2023 07:12:38 GMT  
		Size: 246.1 MB (246079365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm variant v7

```console
$ docker pull rust@sha256:b39c5f27e64b1b5da8b4e9ce47221ccb17371852ce24f88cdd50dc4a7155201a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282607652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83778a9cc65b67d3ead3115054613b3f17fffaa96ed291d1ab23244389fbe181`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:35 GMT
ADD file:8e8c915b4d2c171528ed81da56866395f9a3b0c9260529f0eb2e7df3712cd1f2 in / 
# Thu, 09 Feb 2023 06:11:35 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:23:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Thu, 09 Feb 2023 17:24:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:36dda43b9361bdd95dc7e337cf6cc895b3022cebb556dfc120c6f0a4c3e03877`  
		Last Modified: Thu, 09 Feb 2023 06:18:29 GMT  
		Size: 25.8 MB (25761321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f7af5b8a6b8f28ec136996bca70da7a97ef6dcbf34740c059c40325c709ab3`  
		Last Modified: Thu, 09 Feb 2023 17:29:17 GMT  
		Size: 256.8 MB (256846331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:95a05c437f90c31112e898cded4756f5b5f2d1fe64bb3f6c3d551e6496f378c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335991932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c14fb509a5d1af65da0aa6b9ec67efec569de45b77f0e75ace388e392f389a1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:21 GMT
ADD file:684c8e4c4b00f72eb6c064d1eb2b9c93f03fc3a2904eb861aba1a7f0e2b273a7 in / 
# Thu, 09 Feb 2023 03:58:21 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:39:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Thu, 09 Feb 2023 08:39:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2b995de628a2848dac96f4f608c740b8299d331d61c71872da267f93772c371b`  
		Last Modified: Thu, 09 Feb 2023 04:01:56 GMT  
		Size: 29.1 MB (29065745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f29b5b34bb155eefd11032a3d8dce3896c643dc712ebdf5ca218ea71776d7`  
		Last Modified: Thu, 09 Feb 2023 08:43:02 GMT  
		Size: 306.9 MB (306926187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; 386

```console
$ docker pull rust@sha256:bff785cf12db052cd4e582011991ebcad6df8746012e179d462596efda5c020f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.9 MB (287890907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df08d19b5c3598c98d6b9913625da8e8715c9b51c08933fb6ba7f82a784182c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:25 GMT
ADD file:98fbdac6e3f9c1cf480b4452c3f364942d17c5a8f112d1d48f844c2e43cba09e in / 
# Thu, 09 Feb 2023 05:12:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:10:41 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Thu, 09 Feb 2023 13:11:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:acad3f1f8098c8f067e53067f571a9b121b3011cc77e39d0da11b8bcf7adf2c1`  
		Last Modified: Thu, 09 Feb 2023 05:17:56 GMT  
		Size: 30.1 MB (30057621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e0ee9555e27bfd19024f286946a08b0324a074a1543334841c71be06ed9dc4`  
		Last Modified: Thu, 09 Feb 2023 13:16:58 GMT  
		Size: 257.8 MB (257833286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
