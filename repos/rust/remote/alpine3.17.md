## `rust:alpine3.17`

```console
$ docker pull rust@sha256:caf539826aaca80ac5b49e7c143e6863518517439c83a09c639925783d12ce38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.17` - linux; amd64

```console
$ docker pull rust@sha256:573269348a61483fd36e3049c1379522c60372483d0895dbccc81482e0f835bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272467943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7075cc3f060268e325e901d65ba1a6459429a23eb8aca0f5e13adedb461c79ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:19:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 13 Jul 2023 21:55:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.71.0
# Thu, 13 Jul 2023 21:56:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1692c643fce3f98edc4b47e816dd9dfb0e7bc0e35945cf5f507b0b21027362fd`  
		Last Modified: Thu, 15 Jun 2023 04:20:37 GMT  
		Size: 53.1 MB (53089460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5ab82b7b11e5716f86f29885360718561233d92477492ff52b544769466b32`  
		Last Modified: Thu, 13 Jul 2023 22:02:00 GMT  
		Size: 216.0 MB (216003770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:ba72e40210840174ca2b8c77a6e1fbbe9a4f33826ad166224bf6c5a03817cd3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.4 MB (274429725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35eb55bc07e52af67177bfe15988ce28816bf741149db1096b7c615edeff35b1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:29:03 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 15 Jun 2023 05:29:03 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.70.0
# Thu, 15 Jun 2023 05:29:22 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034e3a5d6ef497cd9d0e1ae19fcaf8b1326b35f5866354a9fbebc84e060333b3`  
		Last Modified: Thu, 15 Jun 2023 05:30:30 GMT  
		Size: 45.6 MB (45608867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f051dffbf03ef242a5f70379f8c371bff190bc21e28164b18061234e162e388c`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 225.6 MB (225559719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
