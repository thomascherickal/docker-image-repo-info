## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:350338510ffea72005818580715f330bd3766ef0f4ddee01d1a8610731c0fce3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:0c8a6ff93fdf8b86902546c8cea1585200b8d46aa251c402345472c888a94b56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.4 MB (178353721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80481926812b1ca18025fb68d541cf640946c76f1fe90c1794b7294341ba41a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 15:12:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 15:12:41 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 15 Nov 2022 15:12:41 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 15:12:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 18 Nov 2022 22:48:10 GMT
ENV JULIA_VERSION=1.9.0-alpha1
# Fri, 18 Nov 2022 22:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-alpha1-linux-x86_64.tar.gz'; 			sha256='c657ed4e792f300d45d1ea5ffb71d052cae4e0d653142b277a3cba4d2cecfd7d'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-alpha1-linux-aarch64.tar.gz'; 			sha256='595451736674c8f2e1cd8be514901cf47043ffc611078c1edcca7d7901ffafb8'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-alpha1-linux-i686.tar.gz'; 			sha256='c8b9312e9b210974a26e9abe3a6d70be9e30f1603a227a11bb2ce1c62351df07'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 18 Nov 2022 22:48:30 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 18 Nov 2022 22:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Nov 2022 22:48:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73274d00911696ee92745d24351073840637e85f3e788218163281a28997d0e`  
		Last Modified: Tue, 15 Nov 2022 15:14:57 GMT  
		Size: 2.4 MB (2427523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9dce66a53430f15f6723a7f558ed9214d0f092e25e7a528fee9981dbc1838`  
		Last Modified: Fri, 18 Nov 2022 22:52:09 GMT  
		Size: 144.5 MB (144513192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79dc923faf9f17fe5a7dbceb4ae868bbf19c124520a28ab05b8575af06ba3f0`  
		Last Modified: Fri, 18 Nov 2022 22:51:46 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:12de2323bc641536255c8830aca231954d39e43044b0562b1ab4245aaa45bd6a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170804791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea07387fbdce3276a226af7d138852a217fde7518ba83f27eebed14b4b91660`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:51:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 03:51:41 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 06 Dec 2022 03:51:41 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 03:51:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 06 Dec 2022 03:51:41 GMT
ENV JULIA_VERSION=1.9.0-alpha1
# Tue, 06 Dec 2022 03:51:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-alpha1-linux-x86_64.tar.gz'; 			sha256='c657ed4e792f300d45d1ea5ffb71d052cae4e0d653142b277a3cba4d2cecfd7d'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-alpha1-linux-aarch64.tar.gz'; 			sha256='595451736674c8f2e1cd8be514901cf47043ffc611078c1edcca7d7901ffafb8'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-alpha1-linux-i686.tar.gz'; 			sha256='c8b9312e9b210974a26e9abe3a6d70be9e30f1603a227a11bb2ce1c62351df07'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 06 Dec 2022 03:51:59 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 03:51:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98701f6087c1d3a7659e32a6d44c77192664fd6fa07cbb399977e76cb6fbf76a`  
		Last Modified: Tue, 06 Dec 2022 03:54:15 GMT  
		Size: 2.4 MB (2415867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660d0c458892f03fc65bf5797340bdcc223adccad28a62359d7ebf7f334dd63c`  
		Last Modified: Tue, 06 Dec 2022 03:54:32 GMT  
		Size: 138.3 MB (138328229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea522580f6dd00d3bb141d9cbc787ff3a936910c2730c07ad545f81603df9a2`  
		Last Modified: Tue, 06 Dec 2022 03:54:15 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:5d2d9bdfe0cb45ccf9101477e8270bb5f75af07f15ba91c24c2c042f631dc6ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176448354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8015944acf7913d0b916cfa5f9d9fd9186529dc0da10339f5c70ecf4f91861f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:58:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:58:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 15 Nov 2022 17:58:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 17:58:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 18 Nov 2022 22:44:57 GMT
ENV JULIA_VERSION=1.9.0-alpha1
# Fri, 18 Nov 2022 22:45:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-alpha1-linux-x86_64.tar.gz'; 			sha256='c657ed4e792f300d45d1ea5ffb71d052cae4e0d653142b277a3cba4d2cecfd7d'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-alpha1-linux-aarch64.tar.gz'; 			sha256='595451736674c8f2e1cd8be514901cf47043ffc611078c1edcca7d7901ffafb8'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-alpha1-linux-i686.tar.gz'; 			sha256='c8b9312e9b210974a26e9abe3a6d70be9e30f1603a227a11bb2ce1c62351df07'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 18 Nov 2022 22:45:19 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 18 Nov 2022 22:45:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Nov 2022 22:45:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a970dc39a82064f89a3db1a8a157503a253665f3b304beee53d089e4285a8aa5`  
		Last Modified: Tue, 15 Nov 2022 18:01:45 GMT  
		Size: 2.3 MB (2327516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b544c33a820a48b0b748c37e1bd1d9bd436b80d897b6204c24f882c347e12`  
		Last Modified: Fri, 18 Nov 2022 22:48:14 GMT  
		Size: 141.7 MB (141727482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e2dfea982d04eab1cfaca61ddb6fff08cb4f319b579bf0bd5d921d65a83c1d`  
		Last Modified: Fri, 18 Nov 2022 22:47:54 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
