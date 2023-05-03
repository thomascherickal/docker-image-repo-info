## `julia:rc-buster`

```console
$ docker pull julia@sha256:311167d1318edbbbb47697943734b2e4ad714b338814d251709a770b8f67608f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:01d1345998cf5f5dd530cb5d4d1a6d72f17a155cc9d88b9b1204098fc22f343e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.2 MB (180152178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2436845200e59e5a0be9aa9c8716900fdea101e79b3d8484894902bc52a698fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:47:16 GMT
ADD file:00bc0eda6d2eb0f8ad4abc654f762ffb9ec7e8d1c95d0cc0e7d0cba176d33e27 in / 
# Tue, 02 May 2023 23:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 04:15:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:15:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 04:15:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 04:15:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 04:15:23 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 04:15:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 04:15:42 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 04:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:15:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:25ff99d195814e98b7ef4708519299d9f177def504f9b718c61eb82c7f0b34be`  
		Last Modified: Tue, 02 May 2023 23:51:01 GMT  
		Size: 27.1 MB (27138959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8239642bfbd72c0ec311c6b3397b94729c8b1aa0a075ba7810daaa2f8084786`  
		Last Modified: Wed, 03 May 2023 04:19:39 GMT  
		Size: 4.5 MB (4472000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7dcb0b03f4d49463775aaa5919b9946366f1f32e7fa149672f01f938dd23af`  
		Last Modified: Wed, 03 May 2023 04:20:00 GMT  
		Size: 148.5 MB (148540847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fdedd319e214114b07f8006fe613144a6afc92b2ec9118ddb68b2f8ada1e7d`  
		Last Modified: Wed, 03 May 2023 04:19:38 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b6164da3a088aaae59667cb1cbd7352340778eab1dd32d9d488562d1e4ad4da0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173154972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1e0dcaffc7b56f0320a86d8ec63995f0a39c6e8f5a3a79269982eae30bf566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 03:38:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:38:31 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:38:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9d51e34e43995301b6f87790745ff2478389d47a336a3dbe05d3e7769181a1`  
		Last Modified: Wed, 03 May 2023 03:40:55 GMT  
		Size: 142.9 MB (142881951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6b4d6106e161bb2a26183c15b5657098535dc303921c7eeeaf025b848d698c`  
		Last Modified: Wed, 03 May 2023 03:40:38 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; 386

```console
$ docker pull julia@sha256:b52b8089ad38b5d507840811a7dd6451679ad1c9104a4f54e7fe4cff949d9bf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178300420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493db3917424668bbc3926b4bd9b50112cfad8bc8115902663938637f7a1a06d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:01:23 GMT
ADD file:b7d2995d8b654298ee7120d8293ac370802e2fda8c311516a581edef93d9e19f in / 
# Wed, 03 May 2023 00:01:24 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:12:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 00:12:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 00:12:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 00:12:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 00:12:06 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 00:12:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 00:12:31 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 00:12:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 00:12:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f1fd7e2201a19e853151f73eb8915b83c7c87b3dae495eef72019fecfbc76b3e`  
		Last Modified: Wed, 03 May 2023 00:05:57 GMT  
		Size: 27.8 MB (27797590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b2d8f6c547476858c61dc17dd055fddaeae5f03ff199633eb47e3514348e6b`  
		Last Modified: Wed, 03 May 2023 00:15:24 GMT  
		Size: 4.6 MB (4623676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17981c10a9de79947a4ec71bba3f307b2e1954fef39806184ab221498b4b697`  
		Last Modified: Wed, 03 May 2023 00:15:53 GMT  
		Size: 145.9 MB (145878783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8dae2e165e09ee9282c8674bea429e427557aa7128ec66402285b34e3364c0`  
		Last Modified: Wed, 03 May 2023 00:15:23 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
