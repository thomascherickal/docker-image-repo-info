## `rust:1-alpine3.15`

```console
$ docker pull rust@sha256:46299b95fb50b86918d69776d611c5a36477b4c8db1ef1358380acbb55fb6140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:787a446dda6a08d20ada523c7400311f51b8d3eb7037e0085bfd6786d8974ae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.4 MB (261350814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f920e55538a58973613f000add723cb5d4a3f96c2d7dd18720faed5a89b809f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:01:15 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 03 Nov 2022 21:00:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.65.0
# Thu, 03 Nov 2022 21:00:39 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ae1636df9a91259b02e35f0f4b6f494afb4dfb9924d408e3556285fc52263c`  
		Last Modified: Fri, 07 Oct 2022 04:02:57 GMT  
		Size: 42.5 MB (42493502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4766b6b0db1a0c57ab6e56bad3c5a1c4fde04604a2d2ee7a12115372203ca`  
		Last Modified: Thu, 03 Nov 2022 21:05:28 GMT  
		Size: 216.0 MB (216033800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0106979c4d32a89a8467e4cf425f054e69e73dccb21734c405e057a2ffe98045
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247401614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7489549aac11a6ab66ff4118e8b08731d6a33c84c3f08febad6a499876e2e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 23:05:37 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 03 Nov 2022 20:09:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.65.0
# Thu, 03 Nov 2022 20:09:17 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6b0e9441be3292c2adb1be6c81c6caaebd816306453325acf9b5934a6f3b8`  
		Last Modified: Tue, 25 Oct 2022 23:10:14 GMT  
		Size: 36.1 MB (36081797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efeed754e9ba871c72c5ce7aa46a358e7c6a19264d6db3621322f41a2efdcf`  
		Last Modified: Thu, 03 Nov 2022 20:14:06 GMT  
		Size: 208.6 MB (208601378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
