## `julia:latest`

```console
$ docker pull julia@sha256:004fee7245d87a62bb0e8c486e500395e558fabb1657ec5d9adb532f32e947b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:7cfa32adea7b4371fe1ae9008ae652ddf7513a8ddadcde9e7178a016d4ccfc01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182753046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd8b425940de708a82a57cdf6ff680c1353a65ad96632a6c0964ccec7a69e58`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 09 Jun 2023 06:30:37 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 06:30:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 09 Jun 2023 06:30:58 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 09 Jun 2023 06:30:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 06:30:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2133ad2a710c5f6d9e003fa21f96aa931db35def0fe2c738bbd8bb7bb5aba3e7`  
		Last Modified: Fri, 09 Jun 2023 06:32:53 GMT  
		Size: 148.9 MB (148922328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd7f2e2902e6e0b6b1fc1cc6c2da9267a9ce56a77c0455a47adf3d398f46df8`  
		Last Modified: Fri, 09 Jun 2023 06:32:32 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:823e703b0880367f29f23b449748cc9e6bb662612f4a9bbefb8f3b7f46d8f89f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175567440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f1a4334b124154a302195a96c740dff10c3d59d49792efc8765c78a52e43ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:22:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:22:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 07:22:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 07:22:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 09 Jun 2023 06:47:03 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 06:47:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 09 Jun 2023 06:47:23 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 09 Jun 2023 06:47:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 06:47:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329488ea119a326bc71c30f0a2609523889ca6ff90a92b88dd627b799bf381c5`  
		Last Modified: Tue, 23 May 2023 07:24:01 GMT  
		Size: 2.4 MB (2414412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b261dd2a6b280456374866eda3477c07abe4baa02b6f3259b4e0deeb343a5052`  
		Last Modified: Fri, 09 Jun 2023 06:48:21 GMT  
		Size: 143.1 MB (143099905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9cfb7a458a3b25784bc1c4aac348fab70e7d53386d3e8d8762d721456aa013`  
		Last Modified: Fri, 09 Jun 2023 06:48:04 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:04273ec5a2e24e2431698c3a8ee3e5346782d564e194872a91a282d368e5a46b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180910486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0727ff984fe07a49653e26b992aac87e2268385b290763a05bc1e9e42f597d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:58 GMT
ADD file:440924fd31c090a7f5e3d36276d17574922eb3e8ececce333fa42f7a95bdd9ce in / 
# Mon, 12 Jun 2023 23:39:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:28:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 13 Jun 2023 04:28:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:28:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 13 Jun 2023 04:28:18 GMT
ENV JULIA_VERSION=1.9.1
# Tue, 13 Jun 2023 04:28:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 13 Jun 2023 04:28:47 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:28:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1646137eb700afc9e891c03fdf28d3f5bc489ef0200fdacc67beee837d48db7d`  
		Last Modified: Mon, 12 Jun 2023 23:47:07 GMT  
		Size: 32.4 MB (32397388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873fa1ac85315b4805888b338f81d9842f04d1e1b1ef970a78a2a2998e8ead92`  
		Last Modified: Tue, 13 Jun 2023 04:30:39 GMT  
		Size: 2.5 MB (2532592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276ae405c9a08cdce42480c181ce9a473a2c3b2ae6f976e6383f4073829777ef`  
		Last Modified: Tue, 13 Jun 2023 04:31:08 GMT  
		Size: 146.0 MB (145980135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d410ec50795029d3c1468392c336d9b17e04595c135f236bb92675f6947fd0e9`  
		Last Modified: Tue, 13 Jun 2023 04:30:38 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:26d287ae0567df47e2de4dd0dab166162ff37de173cfcd71d29681c0bbc412dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171119289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50451cdda0d014f36c7e7fa844e5d5d70b21c36ef344819f37a7c16ef5ab1a71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 09 Jun 2023 08:15:39 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 08:16:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 09 Jun 2023 08:16:27 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 09 Jun 2023 08:16:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 08:16:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa27c06aa782c05b1c72560cf2d1b96dae23f16a2a6f53792defa4e1eba9a816`  
		Last Modified: Fri, 09 Jun 2023 08:17:24 GMT  
		Size: 133.2 MB (133210607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d15628684167a72886e86df6990d37a551ba511e79b307487d60979b0d5c7`  
		Last Modified: Fri, 09 Jun 2023 08:16:47 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:deb179d549707ec99fce6b2305126b7a8ec73e499432a3c0705ea5f8505e8966
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936796937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:726753482e30f8ae6901a05ccbad0578c0409c3661a1b65f387aa9b601ea4518`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 09 Jun 2023 00:34:40 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 00:34:40 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.1-win64.exe
# Fri, 09 Jun 2023 00:34:41 GMT
ENV JULIA_SHA256=e2f105d0ebdcd9a375bfb386bbdacc462effceba0b252f95f27b5660211c8df1
# Fri, 09 Jun 2023 00:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 09 Jun 2023 00:36:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38f406dfeef8d638080fee6dbc302198824cbf29a026eafb6118f8f2355e1a5`  
		Last Modified: Fri, 09 Jun 2023 00:39:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36de2ae5d23482a7549045189e37fcb611f495477deb11c7ad084ece3ee37c8d`  
		Last Modified: Fri, 09 Jun 2023 00:39:46 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5be70deeb5601d9c337e4a8960d71deb910c479f199a1c8638933beb774f8c`  
		Last Modified: Fri, 09 Jun 2023 00:39:46 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39bb8e9865619fd0566b025629352d4a762cf55db993f71900bd979164417c`  
		Last Modified: Fri, 09 Jun 2023 00:40:29 GMT  
		Size: 161.8 MB (161808371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306f3aca6b977181a5a31d77980c8eacf100135e72eb7899317700effa9f8c4e`  
		Last Modified: Fri, 09 Jun 2023 00:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:660c44049dbeddc3a9d1b81d942210fb8c431ccf58e3d25ca80f37365a1f3833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233857811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dfd5df3e4ede56b31608ec07aaaa846008160801338629dd1edec5d6f1fa070`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 09 Jun 2023 00:36:37 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 00:36:38 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.1-win64.exe
# Fri, 09 Jun 2023 00:36:39 GMT
ENV JULIA_SHA256=e2f105d0ebdcd9a375bfb386bbdacc462effceba0b252f95f27b5660211c8df1
# Fri, 09 Jun 2023 00:38:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 09 Jun 2023 00:38:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6843915d8c89b6524c72964ff224097bb26322a44c1b608f18b8db2f52aacf41`  
		Last Modified: Fri, 09 Jun 2023 00:40:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611aab275558eccf1184659a54a5729fa89631bc936628a1d287528f2d08342c`  
		Last Modified: Fri, 09 Jun 2023 00:40:42 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e17a91d283721defc6d239f0c0f5f0f88bfa1b41eaf6d66d07c4f5ee7fcf79`  
		Last Modified: Fri, 09 Jun 2023 00:40:42 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6487525160d3e6300ddab43fdfc2f608e4d523a9a31013d78170cdaf82c555`  
		Last Modified: Fri, 09 Jun 2023 00:41:20 GMT  
		Size: 161.8 MB (161815537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ee81846c7d0e006b37bb927c3a1cdfd26d336c4dce16d17620eb02a70d1d7d`  
		Last Modified: Fri, 09 Jun 2023 00:40:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
