## `rust:1-alpine`

```console
$ docker pull rust@sha256:386495e4f7e356c48b0401e8c0387bfd09171c6cbcea21847bcc68991fb306e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:9e8c9a67a08508d83adca49fd76e756edbc625fc3e1ffc6e0eb48831be7c3bde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.5 MB (249460943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa9cde1d30f2d9a3312d94df8d6764caccd6d9740c39cf7ecb16561615b8cbf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:01:43 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 07 Oct 2022 04:01:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.64.0
# Fri, 07 Oct 2022 04:02:04 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5e6937071324d95490d95db206ab456bf0fb9b56994c8a59f6aab8715bc574`  
		Last Modified: Fri, 07 Oct 2022 04:03:43 GMT  
		Size: 41.4 MB (41443552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a39bb9312fc0a3a47ef4e6c83a4d7ef9cc4c55a9a334ef8bc8264cb84e62f`  
		Last Modified: Fri, 07 Oct 2022 04:04:03 GMT  
		Size: 205.2 MB (205211337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9a9b2122603b5f870b85a7f564925b4bb5a83e4c3b4fc6681c6781eb5575592b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238860370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8427baf3e7072f0ecad3e0d0219ceae37d93e0d4ad5badda17d8eabdf10499`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:25:29 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 22 Sep 2022 18:51:26 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.64.0
# Thu, 22 Sep 2022 18:51:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09504f7cf6d678bdb2f6a52367091e129c8e1c311d9bdfc43e00d796c5a783ee`  
		Last Modified: Wed, 10 Aug 2022 06:28:04 GMT  
		Size: 37.2 MB (37189838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851c4d3ef090799bb7a42b93161871bfb20f0b7fb62acdf3c7c94cc99429f6fa`  
		Last Modified: Thu, 22 Sep 2022 18:57:56 GMT  
		Size: 199.0 MB (198962869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
