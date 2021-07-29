## `rust:slim-bullseye`

```console
$ docker pull rust@sha256:638bf98210c41e0e86ff61604dd1ebada22aa405a40468a2d375b3cac54e869d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:098437d4cc8ffa04dea7976e78b8c14f797519fbe94a5a8900431ebaa61eea71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.9 MB (231902168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4400f6a49c29a54f43c54671ec38756bc90bdbf0a5e8c72ae93bc562d5a02af7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:19 GMT
ADD file:85c9e03c1d9121ebda028664176bf97f6e7a92eeea16af33bce6c2f6a1c4cb02 in / 
# Thu, 22 Jul 2021 00:45:19 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:46:26 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.53.0
# Thu, 22 Jul 2021 17:46:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3ac06a45bc97f56a7ff01e34ad67b7ae7cb0bd2823542469d32bd69a1e5605e8`  
		Last Modified: Thu, 22 Jul 2021 00:49:49 GMT  
		Size: 31.4 MB (31355625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1481203901665481f9574dab719650a44aea2fba8d7159b90356972dd76e78a4`  
		Last Modified: Thu, 22 Jul 2021 17:51:23 GMT  
		Size: 200.5 MB (200546543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:470f0b36fac2a6d24bdf70064fdd608cab35b92f46e785a2b3e535257a6484f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.6 MB (247579724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586276493f9d1e968ec862cfea47473aa21ce078d9cf7ad84ac218ac7d53dd43`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:47 GMT
ADD file:619a96435fb34ae415b7d8a447084f69a98366932e39c923941062bf09d73669 in / 
# Thu, 22 Jul 2021 02:02:48 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 01:57:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.53.0
# Fri, 23 Jul 2021 01:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:05bef09f82badb5e62c3bbcef85c8dff06a3270383173eb2906ed5541afbccc7`  
		Last Modified: Thu, 22 Jul 2021 02:14:54 GMT  
		Size: 26.6 MB (26559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2849c1840f9176e4c247b801a8675a0f08844c3f8106220bf2eeae399a78efe0`  
		Last Modified: Fri, 23 Jul 2021 02:09:49 GMT  
		Size: 221.0 MB (221020298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9d2de1afd63dd4e586acdf6b254210f497a1bfea9fcb577f6003ed38da1695aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278349788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce3d4c9c8119e1191bb6d6c4ee3680b60060c1386d87a1edc43ceeed3368d6f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:6cefc6f682b0bb940ae43c24bc5529327c0ef80c6e6db518107f90cd6293ed33 in / 
# Thu, 22 Jul 2021 00:39:50 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:59:41 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.53.0
# Thu, 22 Jul 2021 13:00:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:beedd8c5cab63478d7358189631ba05b49a730e6e0e188952ea7f9d95327e10b`  
		Last Modified: Thu, 22 Jul 2021 00:44:59 GMT  
		Size: 30.0 MB (30042965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c56332fb4f5891475101d08a0a4642f68d54135ab0c85862444a79745aee73`  
		Last Modified: Thu, 22 Jul 2021 13:05:30 GMT  
		Size: 248.3 MB (248306823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:156877eb79c8b6df9f80ae8c3ae6170f88771313a9a0519fe0d49dd8bc89c562
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.8 MB (296808259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3deabe41f5656ac6530a177bba0dd82c27cf131fa6715d216dd9bed2a8f4bcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:20 GMT
ADD file:7ca10cf9ec4ee7b61d4386a7797bbaa321cfff2a193f3834a78241e8674a2780 in / 
# Thu, 22 Jul 2021 00:39:20 GMT
CMD ["bash"]
# Thu, 29 Jul 2021 18:09:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.54.0
# Thu, 29 Jul 2021 18:11:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0a65268b957466841a0a37aa90035698fb76f15266e0baa350a093adb365ade6`  
		Last Modified: Thu, 22 Jul 2021 00:45:36 GMT  
		Size: 32.4 MB (32369313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2677c087f3dc2ea16b7d5d0d45185292ec203f3f5c5d51dabbc18179d8953`  
		Last Modified: Thu, 29 Jul 2021 18:19:11 GMT  
		Size: 264.4 MB (264438946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
