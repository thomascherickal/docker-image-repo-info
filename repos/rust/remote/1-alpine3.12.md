## `rust:1-alpine3.12`

```console
$ docker pull rust@sha256:374affdc6156d68ac20dbced7a89d809caf70f0328adc015c6db5443bfe14830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:9ff7ca7cd79a60d237f88545bfd4a174535f3c5cb8c5597632162d9e98727eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219688605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeced591196c4bb853022f7e2f4811ebb527d1da65c193c1770372d69d4b9d6f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:59:43 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 Nov 2020 20:31:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.48.0
# Thu, 19 Nov 2020 20:32:10 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c298465e54c33d7619456c0acc3fabb1f1b82649f0b3aae7cd56bed9638be1`  
		Last Modified: Thu, 22 Oct 2020 06:00:45 GMT  
		Size: 47.6 MB (47612902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea20e2680df6410c04905f909aa5964728df5991c6b73edd5137f2c3dd0bb31`  
		Last Modified: Thu, 19 Nov 2020 20:36:14 GMT  
		Size: 169.3 MB (169278843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
