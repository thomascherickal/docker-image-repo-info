## `rust:1-alpine3.18`

```console
$ docker pull rust@sha256:91df043f9c7d48225e64946198f6daabdd0cd9abe2f936d4fe8ca9bc2b1e7101
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.18` - linux; amd64

```console
$ docker pull rust@sha256:f56f2280636a14308a7ffbbf832e06281bc75071a2c2abd9f613d2b5cc0f8828
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270930028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdaec5e2bc3dcdc246d8f1dd9f94704934e2566901b27318d205de13a50c8ddd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:19:33 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 13 Jul 2023 21:56:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.71.0
# Thu, 13 Jul 2023 21:56:30 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6335c2abab213121eb55dff6a0d48faed0716261f80c6e3456e55d37b7e512c8`  
		Last Modified: Thu, 15 Jun 2023 04:21:18 GMT  
		Size: 51.5 MB (51528438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e413d7bdfd29bdcde1ec221397fa78fb275d50ac00fcaf83e2f570309844f75d`  
		Last Modified: Thu, 13 Jul 2023 22:02:42 GMT  
		Size: 216.0 MB (216003711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:8826eee15d75037b04f470c4aa1294ff0a2cbb06fdc14b6c6d6644d97a1ef288
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271904817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7811bcf988f7d232366ebcae84c77b77131b5ec35484ae2b8d912a3cb18dc67a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:29:30 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 13 Jul 2023 22:32:33 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.71.0
# Thu, 13 Jul 2023 22:32:47 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.26.0/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427e5f7304b10c13e04829356b0ed87b97f5a6f29aede9b968ab9a72f9bc910`  
		Last Modified: Thu, 15 Jun 2023 05:31:04 GMT  
		Size: 46.1 MB (46066561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0b407c3776d33a6a354274f9b509a3b68414441dd3401172066133f632540d`  
		Last Modified: Thu, 13 Jul 2023 22:38:39 GMT  
		Size: 222.5 MB (222509005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
