## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:e9b5c8c79c31787cc0653641616c09a8bdd6c1861f19d021848def288cd7aba3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:586a3dddb50160e21d2a894bd0fb195808c787ae31f7126780344b928245253e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177412009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8991eff4893c9e35682bb98b52847f5535e924994ea04d14e39d86b47278c1`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:37:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:37:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 04:37:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 04:37:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 04:37:18 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 04:37:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 04:37:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6cc232341c378ab81793c417267f7bf638f856bae501db76e8852145b7c215`  
		Last Modified: Wed, 11 May 2022 04:40:22 GMT  
		Size: 2.4 MB (2425730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eedc495b914ce00e61ca72914afbec91e35e178b0e46698f17a7d8f725f8ee`  
		Last Modified: Wed, 11 May 2022 04:40:43 GMT  
		Size: 143.6 MB (143606803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0742e039a7dc3c73056e2913eae1c9182723e79246f1fc5117964e9fa410e794
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169427163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd323142fdb6a91484efc64de9e831917910a7e93dffdb2e3e76735cd97fde04`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:20:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:20:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 02:20:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 02:20:55 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 02:20:56 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 02:21:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 02:21:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b6db7251704296faa2ddce3f2ed5530d492e04fc2e34a4be21c7a891b6bf17`  
		Last Modified: Wed, 11 May 2022 02:24:01 GMT  
		Size: 2.2 MB (2208527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22193b27f219088d697207a8973e4bb309b44d49ec2dd7844c21f39fd636fa4`  
		Last Modified: Wed, 11 May 2022 02:24:21 GMT  
		Size: 137.2 MB (137152943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:cf5b308d26ebb79a9b20204cecfc510c3be7ba20c132279aa9ae183cbcf779dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173397587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:167c8ea3e86d76bed770abb2a29c15afa57351dd3027182300d8614959cb7fbc`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:25:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 04:25:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 04:25:39 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 04:25:40 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 04:26:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 04:26:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da3d7a20a87a3dc000dfbfae070e3fe9402e844ce97f575671ece5ae180a376`  
		Last Modified: Wed, 11 May 2022 04:29:19 GMT  
		Size: 2.3 MB (2324111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f765a11666addf62827cf7b9b50c7957959386073d2e1769e3721d652c57566`  
		Last Modified: Wed, 11 May 2022 04:29:41 GMT  
		Size: 138.7 MB (138683700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
