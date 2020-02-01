## `julia:stretch`

```console
$ docker pull julia@sha256:733cffa80bf37f47d4d2de3cb28a40a3e06d86b21de64ee06991829722396939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:stretch` - linux; amd64

```console
$ docker pull julia@sha256:f16498d133d157f29bd5fefe385f482fbfc0c81ef8b889866989dacdc0bd4bae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133452200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b507aa80fa4adf054832444d789687c311b4923b77be08f9567fb2c1de1d93c`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:54:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 Dec 2019 13:54:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:54:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Jan 2020 01:24:05 GMT
ENV JULIA_VERSION=1.3.1
# Tue, 07 Jan 2020 23:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Jan 2020 23:22:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef362d0b91076dc5819a1b925f776504ec063851be5395cadb471b9f3881e`  
		Last Modified: Sat, 28 Dec 2019 13:57:02 GMT  
		Size: 7.6 MB (7555513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71672730cf04ca165569336fedcecf18f18fa7af5bb68b0269336d2cf0104e6d`  
		Last Modified: Tue, 07 Jan 2020 23:23:49 GMT  
		Size: 103.4 MB (103372078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:c96aa5ec4099d65d449554fe6255b743ea25cfab5a1aa847a3cffca734f0f0ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119407020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facee1409787ff6bc644dbfa70a17b807cf03b1a47fae35a99ecd4234ab3e1fa`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 18:35:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 18:35:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 18:35:14 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 18:35:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 18:35:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9840e48d64ced9020e882cefaf8fe5cd26dc391522b6acd18cd09eccad69e07`  
		Last Modified: Sat, 01 Feb 2020 18:39:27 GMT  
		Size: 6.3 MB (6292143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331cb5b72ee568b3cf598db9f378382b4cc073daabb288e06f54994ca3f6ae7`  
		Last Modified: Sat, 01 Feb 2020 18:39:55 GMT  
		Size: 93.8 MB (93803253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:96635540f0bc528b39750e2c03177d4e85a1bb1c080981eb64742ed7d690f4ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113207625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877782fd5d403c41cd3e8bd8175bba4fc79ed5a1a96a15b1715dba7334a7740b`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:09:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 20:09:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 20:09:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 20:09:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 20:10:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 20:10:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa324c835efe4fe5ac3f0b479d4adcb40046011bef28007c8c399f15705879`  
		Last Modified: Sat, 01 Feb 2020 20:13:39 GMT  
		Size: 6.5 MB (6526685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6646730906734e461b2a9c00c1251ff85515f5fa90cc4ad6b6704a8231c55fe`  
		Last Modified: Sat, 01 Feb 2020 20:14:05 GMT  
		Size: 86.3 MB (86295089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; 386

```console
$ docker pull julia@sha256:80af7ef3c4f85fc04cbfa89589a63190f25e1f777664ff9df018dd2def1d5c1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130011823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3b9bf8739ffa78559670835476d3ecc66c66598265715bdc8f0a0841ed6579`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:48:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 01 Feb 2020 17:48:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 17:48:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 01 Feb 2020 17:48:38 GMT
ENV JULIA_VERSION=1.3.1
# Sat, 01 Feb 2020 17:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='faa707c8343780a6fe5eaf13490355e8190acf8e2c189b9e7ecbddb0fa2643ad' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='965c8fab2214f8ce1b3d449d088561a6de61be42543b48c3bbadaed5b02bf824' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e028e64f29faa823557819cf4d5887c0b41c28b5225b60f5f2e5e2f38d453458' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='2cef14e892ac317707b39d2afd9ad57a39fb77445ffb7c461a341a4cdf34141a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 01 Feb 2020 17:48:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3eada1d3458b1595fb3469dbe1f9a16519fe362c19186c018a3f71a94b9b38`  
		Last Modified: Sat, 01 Feb 2020 17:51:37 GMT  
		Size: 7.6 MB (7582401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c4d7471ff49be69dbeb9e909fbfe48ba5fb8252a848e9634ba0b6ec8dbc8`  
		Last Modified: Sat, 01 Feb 2020 17:52:03 GMT  
		Size: 99.3 MB (99277266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
