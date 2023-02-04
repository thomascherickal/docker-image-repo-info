## `rust:slim-bookworm`

```console
$ docker pull rust@sha256:89882bd1868a42f15219627c3ebf0e653bd66afe4155543181e4e39b43b6955b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bookworm` - linux; amd64

```console
$ docker pull rust@sha256:f659eda986b1affa74aa3f4ee24598514b302024447ca1052aa5bf2ca2647c68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.1 MB (275095753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26718ac584fef6d4cc3696232e1e89d9d1cebff0137a647c1d65f71924cedb1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:13 GMT
ADD file:97cee63ee165157eb67c1f292afb7792503022be6e59dc3a4ddace632639ef6a in / 
# Sat, 04 Feb 2023 06:51:13 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:29:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Sat, 04 Feb 2023 13:29:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3b2e7e35590531e4f252f239672d9c3a33ef7c2a6426e2a101b7d12f51413ce6`  
		Last Modified: Sat, 04 Feb 2023 06:55:37 GMT  
		Size: 29.0 MB (29016221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066df457089e66403934167979ae824928fd39aa2012a6f35032667b14229663`  
		Last Modified: Sat, 04 Feb 2023 13:34:43 GMT  
		Size: 246.1 MB (246079532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm variant v7

```console
$ docker pull rust@sha256:44dcad3c435320ef78966288d82ea2c506251ee2a5017e7e0bea021e1805ef81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282620706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c1ba0953593f7a7c450b9d68784177de600c08f553fedeef2119f48fe6e96e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:06 GMT
ADD file:fe4229271bd9ba5c78cfec565c565e2fcbd61b3c50bcad8b5d3a9a27059c47b3 in / 
# Sat, 04 Feb 2023 09:59:06 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:09:34 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Sat, 04 Feb 2023 21:10:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:7ab2a2853da2cf5a541829399203197ca85c39eea6af4bcf1862329542fcbc19`  
		Last Modified: Sat, 04 Feb 2023 10:05:34 GMT  
		Size: 25.8 MB (25774479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df3d219a12e466a89f4e8de1ef28b90826649e8a2249ea8a2351784ec6baa6a`  
		Last Modified: Sat, 04 Feb 2023 21:17:26 GMT  
		Size: 256.8 MB (256846227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:4097e7bfd86279235c7ee0d30cb32842b9a04d378b06c56498d1b9001220f5ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335984543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e817eaac8a9449aa89569eebef58d910b98b96b486902fe46f89fbc48818a948`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:17 GMT
ADD file:2763e979185d4d76d9c09829af4e712ceb87fa0f059891475c43c97700aff882 in / 
# Sat, 04 Feb 2023 06:17:18 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:38:58 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Sat, 04 Feb 2023 17:39:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0d731a398c8953233399260df6d332634065dbf033966c6b8ae92dad011af7ac`  
		Last Modified: Sat, 04 Feb 2023 06:20:47 GMT  
		Size: 29.1 MB (29058213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed825717d8db9367dbd1a083f56051aabc5e0893950ffef4b0e3a2b59f0346d`  
		Last Modified: Sat, 04 Feb 2023 17:45:00 GMT  
		Size: 306.9 MB (306926330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bookworm` - linux; 386

```console
$ docker pull rust@sha256:bb16d2419b099dcf4ce76c6a4aa9dfa28853e432436a705c04f12bab6ce885be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294337992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fbeb4575aa046220f07f77936d34096bae084d97f8fb13f122cb2478e4f574`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:15:39 GMT
ADD file:a62b89896ca7fb2a8ec766b0032aeba42c3652cb9c386a2152f350ea1ef188ee in / 
# Wed, 11 Jan 2023 03:15:40 GMT
CMD ["bash"]
# Thu, 26 Jan 2023 23:44:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.67.0
# Thu, 26 Jan 2023 23:45:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='48c5ecfd1409da93164af20cf4ac2c6f00688b15eb6ba65047f654060c844d85' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='0e0be29c560ad958ba52fcf06b3ea04435cb3cd674fbe11ce7d954093b9504fd' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.25.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:062e1d42805ad2f82a6f2d958d98f73ef51568ebde1c5070441dde2e65c89922`  
		Last Modified: Wed, 11 Jan 2023 03:21:14 GMT  
		Size: 30.1 MB (30052907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efed36bfcee427cd05b6d9c7307bfb2a899c46c50ac3fea4b2e2313f221d2bdc`  
		Last Modified: Thu, 26 Jan 2023 23:51:12 GMT  
		Size: 264.3 MB (264285085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
