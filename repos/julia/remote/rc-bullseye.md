## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:4608442a2d005c162665224f5c948131246209798389bd68bfb7f11cb3eee292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:1e3174d840eda1a366f3c6c25bc8e91b5c8e5e8d2ae5ce5f98a47ed7124d66ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182090698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a0ff04307eb4ba63d5cce658777e0d0ea544a9a03198f72b1aebc4da95d6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:33:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Mar 2023 07:33:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:33:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 01 Mar 2023 07:33:19 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Wed, 01 Mar 2023 07:33:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 01 Mar 2023 07:33:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:33:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:33:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a5daecd3840b3269cf555a93485f58f7c26976c698649b343faeb60e198f76`  
		Last Modified: Wed, 01 Mar 2023 07:36:28 GMT  
		Size: 2.4 MB (2426594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09d6021edd0974cc26b9c96ba3125edd8e042ec3669572fb011131ddb42c87`  
		Last Modified: Wed, 01 Mar 2023 07:36:50 GMT  
		Size: 148.3 MB (148252326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7621c002e0554303eb863e47d7f7a9180bf9d9da7399f1ebb7777b55201cc8c`  
		Last Modified: Wed, 01 Mar 2023 07:36:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:574ec3a53dcc38182d075a3c3c05692a230018f0ff3d3e203e53780a92147f42
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174580406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92d35f1e36df8e2eea0cdc3acc71dd9ae22aaf879570bdd9fb53b4b0a431e59c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:40:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 13:40:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 13:40:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 01:53:43 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 01:54:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 01:54:12 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:54:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3befbc1072899da37ba03cc74c4f850ac9c608aaf7fd9945b690181250505123`  
		Last Modified: Thu, 09 Feb 2023 13:43:09 GMT  
		Size: 2.4 MB (2414195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d69f3e89e543cc34ba93012f542f57fafe16858c0c7ca151a8a55312f6891d`  
		Last Modified: Fri, 10 Feb 2023 01:55:33 GMT  
		Size: 142.1 MB (142103326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5126e2dc2a7e068345a63158cff28a94a72c3354782d7beaa9a4d12bcf8bbd`  
		Last Modified: Fri, 10 Feb 2023 01:55:15 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:0c8b15ba1e938494820a729e9b2281867a229b3794192aa60aba4c3fda74868a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.1 MB (180144598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feddc7d281635cbed61e7426c87735ef9ae45fa64c4c4a67cde6e7b6399a8f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:29:00 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 12:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 12:29:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 01:40:30 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 01:40:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 01:40:57 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be442f0f4ba505349cfe9c32e43ccce6c6d5fe4681dd52f3116fa76df6b79d33`  
		Last Modified: Thu, 09 Feb 2023 12:33:03 GMT  
		Size: 2.3 MB (2326815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd03e724e7a1fafff539a91868920834154209f3d9cdf833252014f55e7db770`  
		Last Modified: Fri, 10 Feb 2023 01:43:05 GMT  
		Size: 145.4 MB (145420530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d00fb72a8c3c2545dff21bcc845c310dcc9e0f57606e4c902d9a962209811`  
		Last Modified: Fri, 10 Feb 2023 01:42:45 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:11a9529569a89bd9b9fa2178c475b8c8347642c9b45ba8ea3efd3fdd568eed4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169346385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c937fd47f43ab77bf29cc979bbbe1692db3dbb9717fc0857e75570a9e56941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:31:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:31:43 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Mar 2023 07:31:43 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:31:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 01 Mar 2023 07:31:44 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Wed, 01 Mar 2023 07:32:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 01 Mar 2023 07:32:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:32:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:32:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb985089da24caae31f3da0a6e6a93223150f39a1eedb005e8b2bd5cc5cbe04`  
		Last Modified: Wed, 01 Mar 2023 07:34:31 GMT  
		Size: 2.6 MB (2627297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5836a2437f8cdec01d0d15dafa337d660b37be5a5a19605b712e036c9a31a58`  
		Last Modified: Wed, 01 Mar 2023 07:35:08 GMT  
		Size: 131.4 MB (131430612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd004806d07aabac6dd2d06f23137f9155fcf10fda803b7db09e06d39c75e978`  
		Last Modified: Wed, 01 Mar 2023 07:34:30 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
