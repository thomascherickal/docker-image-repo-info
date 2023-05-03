## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:eb14474d113e9f09c529e63e593bbe4b22e4f26ba8635897283f9966582e76fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:b548372807ac511318635eb44daede3d3f03ce67ecf079f7d7fc767f2682cb4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182360135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c81dfbeb10eef70db954dad10e6ebe4b37b128e50ce79a749b7df620a564405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 04:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:14:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 04:14:49 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 04:14:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 04:14:50 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 04:15:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 04:15:07 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 04:15:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:15:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4da5f2ad94273f80352cb6898e2347ef78a3570c60ee03d652a6123a571f70`  
		Last Modified: Wed, 03 May 2023 04:19:06 GMT  
		Size: 2.4 MB (2426716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3d8e75dba69e183609cb4154a5ccc346396acefe8f0085752a3754b0c04a2c`  
		Last Modified: Wed, 03 May 2023 04:19:28 GMT  
		Size: 148.5 MB (148529528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53db201c9fbe039f6f87a7002297c6e8e665b1f84fe8369bdf2f57d7286c5f88`  
		Last Modified: Wed, 03 May 2023 04:19:06 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f8cb7947c05202600133c0782074ac851f6b31312a7cf9bd0b666bcb0c37f675
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.3 MB (175349868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ae532b4e96663f6564143c7d93e8fa042424b59bb492b11d5fd35f1b98a706`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 03:37:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:37:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:37:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:37:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91fafe78e42dab6f3764a8d4e612b791f11c2804b4335a5814fd0c794463f6`  
		Last Modified: Wed, 03 May 2023 03:40:25 GMT  
		Size: 142.9 MB (142882436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b9adcc9d0dadaea36b3067725cc3efd8cb6ddf7d92b17d2da1f6280fb2903`  
		Last Modified: Wed, 03 May 2023 03:40:08 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:57ab85c78dc3c12a3af20fda202a7543fbdc1be0c51d8fc80eb294d3251ab506
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180792119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1060b13846829ae3d72c3766b0c777f985afaf37f3dc914489e52463c6160a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:11:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 00:11:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 00:11:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 00:11:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 00:11:25 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 00:11:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc3-linux-x86_64.tar.gz'; 			sha256='d1b2b892e8596ec95cbf7495b8db7815bf7c7b0679c820ea5c8ca2f134be1a7b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc3-linux-aarch64.tar.gz'; 			sha256='0e7b63da2999972cb4a8636670c742d4a6a514bd147da691c05370731fd7f211'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc3-linux-i686.tar.gz'; 			sha256='e8150f48894654fe050efee25a7313b80b55dce48ad26a23f4766b578c3bea3f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc3-linux-ppc64le.tar.gz'; 			sha256='3adda1ffc488bee92d6c969ae3215c90a513c60f99aeb25768f3ebf771f49619'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 00:11:53 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 00:11:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 00:11:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46808a41aeb1079cd8363f7f820c38af5039a3d99ffb031b5b4be27637085da5`  
		Last Modified: Wed, 03 May 2023 00:14:43 GMT  
		Size: 2.5 MB (2532572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f674b07fc92b97d890b4d55e9887134ba113ce6933f7d71b4bf9042e3407dbaf`  
		Last Modified: Wed, 03 May 2023 00:15:12 GMT  
		Size: 145.9 MB (145870964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb09700be157d0b397c0318721d7be6098f66f3329f362e5c8e13f53cddde4f`  
		Last Modified: Wed, 03 May 2023 00:14:42 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:0c18852a3ae42a74c6517490fca281d0f41132e31e0261f9e3a972df4471313e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171153422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134a27b5eb7b567248bf6309ef846165299700a363aff5b0b09311a78111165c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:19:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:19:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 Apr 2023 09:19:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 09:19:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 Apr 2023 09:19:22 GMT
ENV JULIA_VERSION=1.9.0-rc2
# Wed, 12 Apr 2023 09:20:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc2-linux-x86_64.tar.gz'; 			sha256='664f3b50c16c089e9e580958107b4a8e8d1af8206242993601bb3447b4d3541c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc2-linux-aarch64.tar.gz'; 			sha256='2e8325f1c7e14bf2f36e84ef1ed61b51e8a674c8d2cc0f1166b95f3b345e4a3f'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc2-linux-i686.tar.gz'; 			sha256='96bd3db4ab1e846de7f48177521b8c8768bd80e484ed7fd7591a39753f7f9a02'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc2-linux-ppc64le.tar.gz'; 			sha256='4444ecd58bfeed61a969a32cec94df8860cdb02314bc09c10af6958fdd5d4c31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 Apr 2023 09:20:24 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:20:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 09:20:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21139c90c7454c3c608059c774bd8d3ee2642c3ee8da2adab1962a2b62581b8`  
		Last Modified: Wed, 12 Apr 2023 09:22:21 GMT  
		Size: 2.6 MB (2627375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82df6fa1b83af9c04bb3d6c5f427f96b34edb589391e0f6c128e9af33de2a21b`  
		Last Modified: Wed, 12 Apr 2023 09:22:58 GMT  
		Size: 133.2 MB (133233677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007b0f2c3ca147214b5a80d19726543dfb3dfda35e72148c6668aceab00fcbe5`  
		Last Modified: Wed, 12 Apr 2023 09:22:20 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
