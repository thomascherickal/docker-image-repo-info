## `julia:rc-bookworm`

```console
$ docker pull julia@sha256:a6c175c6aa6d363255191515147e84b85c0b7f68755b98c9d8979dfb40409566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:3e2b3ec8a7726c20788e5824d7be0da7080eb97d781b2e0a8da169e433830918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208910026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a64b41b1e57af519f1dee2e78a72be65c70fa5682ef06a0d3a930dcbd06fcec0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:56:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:56:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:56:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:56:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 11 Jul 2023 22:25:45 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Tue, 11 Jul 2023 22:26:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 11 Jul 2023 22:26:09 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 11 Jul 2023 22:26:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 22:26:09 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06944e2a3b3efedafb03a42dd3d3c9211b5e729038eacb6fa0a2ebf03a737834`  
		Last Modified: Tue, 04 Jul 2023 12:58:53 GMT  
		Size: 5.7 MB (5695811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dcdd997dfee97ca39bd89249f3ac64845e17dd24d975cd43e0953b7bf1d6c0`  
		Last Modified: Tue, 11 Jul 2023 22:28:37 GMT  
		Size: 174.1 MB (174089013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad024bc88d948519290e09fe3a0224e9c32921e9d063be9b73c4202d47a3279`  
		Last Modified: Tue, 11 Jul 2023 22:28:12 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:3999c77e0f3a1f4769e163d2bf4e7057840bb5f4d5a6d528d91da8e758f45d6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203343328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b264368dd4c9ad5fa4c97878e5e6563a7f17b4b7389ac80960fb6a1fb5e81d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:52:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:52:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:52:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 11 Jul 2023 22:44:50 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Tue, 11 Jul 2023 22:45:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 11 Jul 2023 22:45:15 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 11 Jul 2023 22:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 22:45:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579fe3ef433e4417135885378c889772d9214a97384ecddb087c5cd2aec31fc9`  
		Last Modified: Tue, 04 Jul 2023 03:54:38 GMT  
		Size: 5.5 MB (5526511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4345876a92abcbe915cdbfe7fabba15880cd427a5a4bbd340482c475dc8bf9`  
		Last Modified: Tue, 11 Jul 2023 22:46:29 GMT  
		Size: 168.7 MB (168663986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4418b1fb92bee6d3cca4454674e10ce0475e050e3405f2b3b383a6381522698c`  
		Last Modified: Tue, 11 Jul 2023 22:46:09 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; 386

```console
$ docker pull julia@sha256:6a836ce09587063742a452ef0901a51555659635831963901cfe32eb7e763eb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196230609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b0ec978b378d341a87b15e47381af74e6fdd9a24eba5c87ae58e0b15110883`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:36 GMT
ADD file:441addef37edd5da10ca045fe9cc7863b0785f468d83c3884456efd567e97536 in / 
# Tue, 04 Jul 2023 01:38:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:52:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:52:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:52:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 11 Jul 2023 22:40:26 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Tue, 11 Jul 2023 22:40:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 11 Jul 2023 22:41:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 11 Jul 2023 22:41:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 22:41:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7d4b098d102e200415126181e2b6aae752738430f2ed6a601f84baf29e2f7d01`  
		Last Modified: Tue, 04 Jul 2023 01:43:28 GMT  
		Size: 30.1 MB (30140746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1237bf9b06dc0a5e2ee3eef76817ae8e81fa1e6360bb86f64feb1916b95a63`  
		Last Modified: Tue, 04 Jul 2023 08:54:59 GMT  
		Size: 5.9 MB (5854604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2052df6fdff317d4ff4c98f1619dec3e1e6a4a1ca4ee8ec965480e298299e466`  
		Last Modified: Tue, 11 Jul 2023 22:42:38 GMT  
		Size: 160.2 MB (160234886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1117e2c6bbba96ff8f67b54d413639a2c414fe5017f58b99ba93908820f2487`  
		Last Modified: Tue, 11 Jul 2023 22:42:05 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:c033a00523c1b65c919a338855307e6513aa59ffcd70014b51348ac20d81523a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197890608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641bec901192868c323b0c3cc8e4073f8604261f00192e9237cff6446846df20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:40:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:40:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 11 Jul 2023 22:19:46 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Tue, 11 Jul 2023 22:20:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 11 Jul 2023 22:20:45 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 11 Jul 2023 22:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 22:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e00614d6b132be437f8e5dd49964584196c1794d22317ffbd448602456fd920`  
		Last Modified: Tue, 04 Jul 2023 06:43:46 GMT  
		Size: 6.2 MB (6229887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f71477eaf8db4882ea7235588d2d4a2b11daa594d350a2a852ab69f5959794`  
		Last Modified: Tue, 11 Jul 2023 22:23:24 GMT  
		Size: 158.5 MB (158543633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a62d83e4c5c32050d5f745951f943a19aec8f0668d21601068034366c893f2e`  
		Last Modified: Tue, 11 Jul 2023 22:22:40 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
