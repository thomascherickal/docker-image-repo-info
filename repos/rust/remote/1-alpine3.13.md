## `rust:1-alpine3.13`

```console
$ docker pull rust@sha256:5280ec3be86b0b81da654e7c019ab3ec10a7e7e8556dfe5e02bdf2276d11be04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.13` - linux; amd64

```console
$ docker pull rust@sha256:c4863327ef8c89bb3ebe7db2f0ed6e06c8d3ef41dbfe28fbc0b4e6362407747b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (247977671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15d1ad3d3430e4ead86257997231c1eeda9b743674477612e51bf656c265fb6e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 00:56:34 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 12 Feb 2021 00:56:35 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Fri, 12 Feb 2021 00:56:58 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c16aa051e0917f545e52351ee037d05a577b8e616db1d66cab42261624cdbd`  
		Last Modified: Fri, 12 Feb 2021 00:59:45 GMT  
		Size: 42.2 MB (42173680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c45b940af240552080d81056a4429cafd3872f111b765f97c3b6acb66545604`  
		Last Modified: Fri, 12 Feb 2021 01:00:13 GMT  
		Size: 203.0 MB (202992670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:4edaa5106433cf4f28be6fdee4a3643769cff838b16d387b2cad9e5fb07ec356
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223902219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac698b778d4fc462c48d4717e6f93ae5ff2dd41d72ff3faf2f4c62984a8471c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 01:04:11 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 12 Feb 2021 01:04:12 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Fri, 12 Feb 2021 01:04:33 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df52b864c5ea8683e3f37ad0ac769a5a4cb31728797fdeb457d4722189106c6`  
		Last Modified: Fri, 12 Feb 2021 01:08:27 GMT  
		Size: 35.9 MB (35928145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cb0df2c7ff06ef5f4615fe6d4ed4fe8c6d649e6963ea0b3e92d5daa084967f`  
		Last Modified: Fri, 12 Feb 2021 01:09:02 GMT  
		Size: 185.3 MB (185262813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
