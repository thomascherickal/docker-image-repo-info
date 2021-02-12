## `rust:1-alpine3.12`

```console
$ docker pull rust@sha256:8c4cac220152297b0549d5eed64dff773698caab0a5736869aaeca0a35f7e7f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:f7cabcc370a135407712f4b4374ce9127e5394a6805dca7c872aab444419a25b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253404779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc710353d61c108bed6c271f3293d7d145ad425599c8c3a8c859d151f60d159`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 15:05:24 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 12 Feb 2021 00:55:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Fri, 12 Feb 2021 00:56:22 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7443742b0810d88d0929d41931d7dc9ae6952a907581f6296164982e5285a57c`  
		Last Modified: Thu, 17 Dec 2020 15:07:49 GMT  
		Size: 47.6 MB (47612978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c433f73194e70485fe2efa4dadeeba0b1d59a403a9a1d565d6946a5332ed7`  
		Last Modified: Fri, 12 Feb 2021 00:59:26 GMT  
		Size: 203.0 MB (202992735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1d158f5685fe446b054b37aaffcc6c5ae4ea9152be3a6782539f150b94b4d4ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226533228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb5a63de5740c705a273bbbdcaeb56b41cdda8c44bb53ee9f7234f99b2a8f3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 31 Dec 2020 19:46:57 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 12 Feb 2021 01:03:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.50.0
# Fri, 12 Feb 2021 01:03:56 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='05c5c05ec76671d73645aac3afbccf2187352fce7e46fc85be859f52a42797f6' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='6a8a480d8d9e7f8c6979d7f8b12bc59da13db67970f7b13161ff409f0a771213' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.23.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562371de7ae1ed2e620bf195edf2b1973a49eadff6f2e57f53587df3c9b11515`  
		Last Modified: Thu, 31 Dec 2020 19:50:35 GMT  
		Size: 38.6 MB (38561454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dacbd10c30e07c2f1fd072aedc805fdcf368ee8102c47c55f50739fc27720be`  
		Last Modified: Fri, 12 Feb 2021 01:08:08 GMT  
		Size: 185.3 MB (185262726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
