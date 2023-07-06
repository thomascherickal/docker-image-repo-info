<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.17`](#julia1-alpine317)
-	[`julia:1-alpine3.18`](#julia1-alpine318)
-	[`julia:1-bookworm`](#julia1-bookworm)
-	[`julia:1-bullseye`](#julia1-bullseye)
-	[`julia:1-windowsservercore`](#julia1-windowsservercore)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2022`](#julia1-windowsservercore-ltsc2022)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6-alpine`](#julia16-alpine)
-	[`julia:1.6-alpine3.17`](#julia16-alpine317)
-	[`julia:1.6-alpine3.18`](#julia16-alpine318)
-	[`julia:1.6-bookworm`](#julia16-bookworm)
-	[`julia:1.6-bullseye`](#julia16-bullseye)
-	[`julia:1.6-windowsservercore`](#julia16-windowsservercore)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2022`](#julia16-windowsservercore-ltsc2022)
-	[`julia:1.6.7`](#julia167)
-	[`julia:1.6.7-alpine`](#julia167-alpine)
-	[`julia:1.6.7-alpine3.17`](#julia167-alpine317)
-	[`julia:1.6.7-alpine3.18`](#julia167-alpine318)
-	[`julia:1.6.7-bookworm`](#julia167-bookworm)
-	[`julia:1.6.7-bullseye`](#julia167-bullseye)
-	[`julia:1.6.7-windowsservercore`](#julia167-windowsservercore)
-	[`julia:1.6.7-windowsservercore-1809`](#julia167-windowsservercore-1809)
-	[`julia:1.6.7-windowsservercore-ltsc2022`](#julia167-windowsservercore-ltsc2022)
-	[`julia:1.9`](#julia19)
-	[`julia:1.9-alpine`](#julia19-alpine)
-	[`julia:1.9-alpine3.17`](#julia19-alpine317)
-	[`julia:1.9-alpine3.18`](#julia19-alpine318)
-	[`julia:1.9-bookworm`](#julia19-bookworm)
-	[`julia:1.9-bullseye`](#julia19-bullseye)
-	[`julia:1.9-windowsservercore`](#julia19-windowsservercore)
-	[`julia:1.9-windowsservercore-1809`](#julia19-windowsservercore-1809)
-	[`julia:1.9-windowsservercore-ltsc2022`](#julia19-windowsservercore-ltsc2022)
-	[`julia:1.9.2`](#julia192)
-	[`julia:1.9.2-alpine`](#julia192-alpine)
-	[`julia:1.9.2-alpine3.17`](#julia192-alpine317)
-	[`julia:1.9.2-alpine3.18`](#julia192-alpine318)
-	[`julia:1.9.2-bookworm`](#julia192-bookworm)
-	[`julia:1.9.2-bullseye`](#julia192-bullseye)
-	[`julia:1.9.2-windowsservercore`](#julia192-windowsservercore)
-	[`julia:1.9.2-windowsservercore-1809`](#julia192-windowsservercore-1809)
-	[`julia:1.9.2-windowsservercore-ltsc2022`](#julia192-windowsservercore-ltsc2022)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.17`](#juliaalpine317)
-	[`julia:alpine3.18`](#juliaalpine318)
-	[`julia:bookworm`](#juliabookworm)
-	[`julia:bullseye`](#juliabullseye)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore`](#juliawindowsservercore)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2022`](#juliawindowsservercore-ltsc2022)

## `julia:1`

```console
$ docker pull julia@sha256:e95993d17016c2df34d63bc7d2a0673e69f92d06cb1e393f0217894a874a8b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.17`

```console
$ docker pull julia@sha256:d5c4035b68e660e213772c08e46a9efb70895aa397f664dda89344cf1b066bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2e3b7d449f63f6759404bf3e414164559d8b56d076ae10a7d9493b153dccefca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154517691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fecf32bc21e8f19277b73f5ae1fbfbb7f61996eec72e6db0b3c341c0d83c35f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:25:01 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:25:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:25:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:25:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aca3cbabb864e81b14b1cf75dee6cb4a5c034a5c4d529b4dd548c708ad7585`  
		Last Modified: Thu, 06 Jul 2023 20:28:15 GMT  
		Size: 151.1 MB (151142605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5584a8659f45d6418de9bea871a53ad36743c215f9cdcc65b2bf41c93df8f8eb`  
		Last Modified: Thu, 06 Jul 2023 20:27:53 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.18`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-bookworm`

```console
$ docker pull julia@sha256:9a8f501b64033b3267f3e20254b9dd760c27c41b3df74dbc78f65c7a3eb92769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bookworm` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-bullseye`

```console
$ docker pull julia@sha256:b8c7552ed06d657777a1cbe5d0b8e3612f50c5b5fa481a86c8eb97fb46e0e75c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:aaeaaa3d7dbaef6d2ec4cc5a7411ec9a9c0c69b174af53cdc0cdf3c35b7cf7b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182827655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8faa5f3694dc11c54608231a241f0e22b0ab343df1cf658181ccb08fa52feea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:38 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5ba2316d48362d9eb272a6551eafd1093f623c54f771aa94b0505319d83801`  
		Last Modified: Thu, 06 Jul 2023 20:26:56 GMT  
		Size: 149.0 MB (148983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbbc851898f4fe7e45d809b9c5b6e29ae7775d8e4da389a76824adb60cfecf4`  
		Last Modified: Thu, 06 Jul 2023 20:26:34 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:421f13803f4850ea52d09920f12147c018596841b7009a896bf6ad35c358bd5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175594642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a550b8c8f1775b3a11fad42cae90fe5af0c2d6e92b0cbd293277cbe54a7af289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:54:08 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:54:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb4f341423d35b379731ed8751938166da78d0156cc03ee3e5ac5c50215add`  
		Last Modified: Thu, 06 Jul 2023 19:55:35 GMT  
		Size: 143.1 MB (143116901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae40477f57ed335e0bcea787cfc74221033f2504aef4c8e2c7f9979ee3f367`  
		Last Modified: Thu, 06 Jul 2023 19:55:18 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ce5938fb6fe97c2bc0f89fec3e1137d9e577b5d1689fc20308a6cbe4dca01d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172541142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7162832f8861471c6e00bc1df0a84f210b183eeae363bb5568d685e476e30b04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:41:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:44 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb637a0e859dfa93ee87c91ea9411f73f8f3ac5b7dcf5cd93df78c651f0fcba4`  
		Last Modified: Thu, 06 Jul 2023 19:43:16 GMT  
		Size: 137.6 MB (137610741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee123d90de401331f01e2bfcde57c1b8f99c35ae344edf4da35365cfd22eaf`  
		Last Modified: Thu, 06 Jul 2023 19:42:48 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:41c46f675bfea61c7cfa392e0ae5e62e86121a60e929048ce44383fd3a305b2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171241827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97355cbc9364a46b4490c47295e6169f0825bc3c623e868573f56c96f9862aa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:33 GMT
ADD file:37fa020aca7253d41d395ed529c38db73caaa4da098754836244552f65fa7d5d in / 
# Tue, 04 Jul 2023 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:42:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:42:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:42:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:42:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:17:48 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:18:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:18:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:18:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:147bb8b5828c99cd6b07d252d2987490463c142099eaa0815025685f8fa4f3d8`  
		Last Modified: Tue, 04 Jul 2023 01:25:40 GMT  
		Size: 35.3 MB (35291082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6ddbab4eda0628b3aa67cecb27fb39624b779814fe84d9f47de75724b8f22f`  
		Last Modified: Tue, 04 Jul 2023 06:44:40 GMT  
		Size: 2.6 MB (2627602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78898475b67599608955aad6821eaf3eea34dbb639469120507a4eac042c28`  
		Last Modified: Thu, 06 Jul 2023 20:20:34 GMT  
		Size: 133.3 MB (133322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45330019a76b147b8f737bb6f568c7828a1120f0aa94bd6c0d244df64d36dba0`  
		Last Modified: Thu, 06 Jul 2023 20:19:58 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore`

```console
$ docker pull julia@sha256:81c6d8b118fd0fab2967dc9187bc3c31a5d6e016197563adacf1c0aa1a634078
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:c72611e6cce79bcf49a5cd17fe3caeecfab0852fee938a219ef20302f8b5c0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:e4fc96d43a5cead4e8df2c841d75020c9d9b7b6f2e680e981b531ff190a47559
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:ece83eb0ca8812e40c9374a239ff80566b10b240fe9a1b649d3b90eb9e82cb4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:e5e1d337433439da417b79ca51cd63698fc48e7ff032b6b1f1c46b3b808570c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157448493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff62465e425cd7947df6c2eaa5231b1395cef69314b3b07051e72b3395b7d1`
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
# Tue, 04 Jul 2023 12:57:46 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:01 GMT
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
	-	`sha256:3d5c0da1f8ee41aadc9bf9f49aef04ca0203aac6d219a9c528168488834e2ebd`  
		Last Modified: Tue, 04 Jul 2023 13:00:22 GMT  
		Size: 122.6 MB (122627479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26872efe14570e5349d5d332f0adeac8e1e17930860e3fc68ce81a03e9b8f9e9`  
		Last Modified: Tue, 04 Jul 2023 13:00:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:2ab09c60ea80307493ca999611b6dbdcfd7fecdab736caf8dd973aadb0070a5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143294057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81ef026a69b9806a304414ff48ee16616123a66928838e8631c7095241ce4945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:26:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:26:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:26:59 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db77a978ab7f92a239b0408105fd78a65e1664b8e8ece6366e8a47461a506e24`  
		Last Modified: Tue, 04 Jul 2023 06:27:51 GMT  
		Size: 4.8 MB (4816363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43958bd99698dbd25abd055f5a29a7f2c249b36f8d595f7901ff169784cd6b9`  
		Last Modified: Tue, 04 Jul 2023 06:28:12 GMT  
		Size: 113.7 MB (113676056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621eaefc355c8ff33315977f36c564b56529b9f878e8af23f138e95673d129e`  
		Last Modified: Tue, 04 Jul 2023 06:27:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5056202c38c8e3b88b20615d41c93fc958d6bf4a80bcc1a3b53765c232df6e3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.1 MB (151095312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd94729d9ee9304a370b1ba5ac646b8faaa650776487165626207b6276dbe975`
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
# Tue, 04 Jul 2023 03:53:42 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:01 GMT
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
	-	`sha256:41a4dc5dccca253e2aa8ac911ac7815d685a43fa9ed3a0ae94dbf2abaceaff29`  
		Last Modified: Tue, 04 Jul 2023 03:55:51 GMT  
		Size: 116.4 MB (116415969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc61605bab7c03fce76d6926e712aaefc9928e00025d64c796e4e222b5f7ab2`  
		Last Modified: Tue, 04 Jul 2023 03:55:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:c03e763abd1ce1958730a814a20c7a1ce1435e64fef6695af23588eed2fc178f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156290528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e984d299c4a75d49225c3fbc5e3e291017be7fbb09b8f195ebbc6966fec38d94`
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
# Tue, 04 Jul 2023 08:53:53 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:17 GMT
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
	-	`sha256:efc2306d7bacc61b98692dfff1b673341c9e1fd92384e8ec9ef718fbfb73e54a`  
		Last Modified: Tue, 04 Jul 2023 08:56:44 GMT  
		Size: 120.3 MB (120294809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8544337e3567a9768a97fd7d17b05eab7360c12bdb92a9140524585c2fc14be4`  
		Last Modified: Tue, 04 Jul 2023 08:56:21 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:48212100c7b69a0a5ea68d7d375452ad169a85eafd87c740062e143597e6b95a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:f9db4933a708ae86f0e89f04dfb77be6f48fec073b2e1bd548ff7e07755b927f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e8f8c6310b13b584db3297d92a85b05e756817dd55cea187a7f4b3c1c981d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:14:58 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b14b8c15ddbe32a9d67d670852149497149928cac8d6db33b30b70d28afdf0a`  
		Last Modified: Thu, 15 Jun 2023 00:17:43 GMT  
		Size: 121.8 MB (121829514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3972cf1468f8db4d4ba693b4511092b7c9e32fc1a6413bad0b1f7064da70d`  
		Last Modified: Thu, 15 Jun 2023 00:17:26 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.17`

```console
$ docker pull julia@sha256:92185c71acc5290d8dbc4d23deee54a3cd0ac8f2b51a32dc5261df9362615c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2df858e1d333ccf9a097e2b810600bf881651f8b5316a05dca5e62968fb4c299
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125204631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9242533c211a85926b20781d026374068fd209172cc69dcd40dfe497c8a0dce2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:15:19 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:31 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1bec9354fb7c25c6a8f40a4568daf57e0f9a4a5c965036793baa6be8557fb`  
		Last Modified: Thu, 15 Jun 2023 00:18:13 GMT  
		Size: 121.8 MB (121829545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca91bfa84b37afae43457469b7b6ed30faf890c63620fcfb04007180d83f5e4e`  
		Last Modified: Thu, 15 Jun 2023 00:17:56 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.18`

```console
$ docker pull julia@sha256:48212100c7b69a0a5ea68d7d375452ad169a85eafd87c740062e143597e6b95a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:f9db4933a708ae86f0e89f04dfb77be6f48fec073b2e1bd548ff7e07755b927f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e8f8c6310b13b584db3297d92a85b05e756817dd55cea187a7f4b3c1c981d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:14:58 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b14b8c15ddbe32a9d67d670852149497149928cac8d6db33b30b70d28afdf0a`  
		Last Modified: Thu, 15 Jun 2023 00:17:43 GMT  
		Size: 121.8 MB (121829514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3972cf1468f8db4d4ba693b4511092b7c9e32fc1a6413bad0b1f7064da70d`  
		Last Modified: Thu, 15 Jun 2023 00:17:26 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-bookworm`

```console
$ docker pull julia@sha256:81290e372fb84a653b1ceb07a2e13f93af6dda3f5197191cde95ace5a08a5bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:e5e1d337433439da417b79ca51cd63698fc48e7ff032b6b1f1c46b3b808570c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157448493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff62465e425cd7947df6c2eaa5231b1395cef69314b3b07051e72b3395b7d1`
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
# Tue, 04 Jul 2023 12:57:46 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:01 GMT
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
	-	`sha256:3d5c0da1f8ee41aadc9bf9f49aef04ca0203aac6d219a9c528168488834e2ebd`  
		Last Modified: Tue, 04 Jul 2023 13:00:22 GMT  
		Size: 122.6 MB (122627479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26872efe14570e5349d5d332f0adeac8e1e17930860e3fc68ce81a03e9b8f9e9`  
		Last Modified: Tue, 04 Jul 2023 13:00:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bookworm` - linux; arm variant v7

```console
$ docker pull julia@sha256:2ab09c60ea80307493ca999611b6dbdcfd7fecdab736caf8dd973aadb0070a5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143294057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81ef026a69b9806a304414ff48ee16616123a66928838e8631c7095241ce4945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:26:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:26:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:26:59 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db77a978ab7f92a239b0408105fd78a65e1664b8e8ece6366e8a47461a506e24`  
		Last Modified: Tue, 04 Jul 2023 06:27:51 GMT  
		Size: 4.8 MB (4816363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43958bd99698dbd25abd055f5a29a7f2c249b36f8d595f7901ff169784cd6b9`  
		Last Modified: Tue, 04 Jul 2023 06:28:12 GMT  
		Size: 113.7 MB (113676056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621eaefc355c8ff33315977f36c564b56529b9f878e8af23f138e95673d129e`  
		Last Modified: Tue, 04 Jul 2023 06:27:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5056202c38c8e3b88b20615d41c93fc958d6bf4a80bcc1a3b53765c232df6e3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.1 MB (151095312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd94729d9ee9304a370b1ba5ac646b8faaa650776487165626207b6276dbe975`
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
# Tue, 04 Jul 2023 03:53:42 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:01 GMT
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
	-	`sha256:41a4dc5dccca253e2aa8ac911ac7815d685a43fa9ed3a0ae94dbf2abaceaff29`  
		Last Modified: Tue, 04 Jul 2023 03:55:51 GMT  
		Size: 116.4 MB (116415969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc61605bab7c03fce76d6926e712aaefc9928e00025d64c796e4e222b5f7ab2`  
		Last Modified: Tue, 04 Jul 2023 03:55:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bookworm` - linux; 386

```console
$ docker pull julia@sha256:c03e763abd1ce1958730a814a20c7a1ce1435e64fef6695af23588eed2fc178f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156290528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e984d299c4a75d49225c3fbc5e3e291017be7fbb09b8f195ebbc6966fec38d94`
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
# Tue, 04 Jul 2023 08:53:53 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:17 GMT
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
	-	`sha256:efc2306d7bacc61b98692dfff1b673341c9e1fd92384e8ec9ef718fbfb73e54a`  
		Last Modified: Tue, 04 Jul 2023 08:56:44 GMT  
		Size: 120.3 MB (120294809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8544337e3567a9768a97fd7d17b05eab7360c12bdb92a9140524585c2fc14be4`  
		Last Modified: Tue, 04 Jul 2023 08:56:21 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-bullseye`

```console
$ docker pull julia@sha256:bf24ff1eb752d5b837334acad7cd8c95718f6e976b8f115c9fa549eabc390a1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:2eaa299a228888695a12824ab8416a838ac14319f1f3fd53308946118de74b18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156484503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdea7ff13328a8e22bc36bdc348ad705b51930de3c3674ae90b4ce531cb131ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 12:58:05 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:21 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef54198d58cd5f9737d61a032200003a68a1eeabe41f38661bde18f23ccfac44`  
		Last Modified: Tue, 04 Jul 2023 13:00:48 GMT  
		Size: 122.6 MB (122640066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71befbca109de1b0e96c2ebd0bda47988c67bbdb2219eca79f27c3bed4d05def`  
		Last Modified: Tue, 04 Jul 2023 13:00:30 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:5507fc803951e5d7d6bc3ab131884db671da38de9b9e0ecbb8aff568bb2dd7b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142495992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415357620180759f54d516711f562be5b3583e8692074e914b4f16a1744d8c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:27:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:27:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:27:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7a9ee38b3bace42d79860e8d0f20a27ab6851a4c4d931a4fe5d7c513d6aea`  
		Last Modified: Tue, 04 Jul 2023 06:28:21 GMT  
		Size: 2.2 MB (2228939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16543aa34ebb99eee649999641723c251c7d3b571726b7c585e71fce686bbd4`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 113.7 MB (113687926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb00013048d915815a9aae6a11e9969470bbea37f34b3ac2d165d89b55f1d6`  
		Last Modified: Tue, 04 Jul 2023 06:28:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1b45c09df9ae2097879d4eb1376a32a9fa70cfc3a7309d03e2c831c8d28126d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148906138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4078b7c4a11b4a16232f9835a35fc1b634a5264fb0b37cfc4286b364450829cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 03:54:05 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:54:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:21 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c6c16eb8611d5f73aaf1004452d08d9a59e6fed1f4c22e99fdb2d4ac17acd9`  
		Last Modified: Tue, 04 Jul 2023 03:56:12 GMT  
		Size: 116.4 MB (116428395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631d3696ceee8180e5f6de536e4482cf1982bd3116c4c61b4aea079df1d4494f`  
		Last Modified: Tue, 04 Jul 2023 03:55:59 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; 386

```console
$ docker pull julia@sha256:6ee273b3181c594cc0f03d355b6a75b4cf1ef10a188c411fce09a713f46cd6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155237947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad331954ef6fcbd49eb58fcabd8b718144e4c13efbb6c8cd4fffe3d8c5229cb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 08:54:21 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:42 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78c00973a02bf0768ad9012c721ff22e529b3ef7ed44a69cbf8b0de03866f22`  
		Last Modified: Tue, 04 Jul 2023 08:57:19 GMT  
		Size: 120.3 MB (120307546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ca4fd5e402f51c93f9c8ff5bc51da54aebdfafb3ef3d88bada6cebf1acad7`  
		Last Modified: Tue, 04 Jul 2023 08:56:55 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore`

```console
$ docker pull julia@sha256:9883f88d57cdcca134f39df309332d01684fee43969649dd5f6866877d651768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:f069b3a89018b1362a9b10b945fd96a2a8bf830ab182606fa766fbb8b45cc81e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:a72a9850d0f754213d8fa95591301d2217a4ea33799489b4cb4be82a2998ceb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:1.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7`

```console
$ docker pull julia@sha256:ece83eb0ca8812e40c9374a239ff80566b10b240fe9a1b649d3b90eb9e82cb4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6.7` - linux; amd64

```console
$ docker pull julia@sha256:e5e1d337433439da417b79ca51cd63698fc48e7ff032b6b1f1c46b3b808570c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157448493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff62465e425cd7947df6c2eaa5231b1395cef69314b3b07051e72b3395b7d1`
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
# Tue, 04 Jul 2023 12:57:46 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:01 GMT
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
	-	`sha256:3d5c0da1f8ee41aadc9bf9f49aef04ca0203aac6d219a9c528168488834e2ebd`  
		Last Modified: Tue, 04 Jul 2023 13:00:22 GMT  
		Size: 122.6 MB (122627479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26872efe14570e5349d5d332f0adeac8e1e17930860e3fc68ce81a03e9b8f9e9`  
		Last Modified: Tue, 04 Jul 2023 13:00:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm variant v7

```console
$ docker pull julia@sha256:2ab09c60ea80307493ca999611b6dbdcfd7fecdab736caf8dd973aadb0070a5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143294057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81ef026a69b9806a304414ff48ee16616123a66928838e8631c7095241ce4945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:26:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:26:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:26:59 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db77a978ab7f92a239b0408105fd78a65e1664b8e8ece6366e8a47461a506e24`  
		Last Modified: Tue, 04 Jul 2023 06:27:51 GMT  
		Size: 4.8 MB (4816363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43958bd99698dbd25abd055f5a29a7f2c249b36f8d595f7901ff169784cd6b9`  
		Last Modified: Tue, 04 Jul 2023 06:28:12 GMT  
		Size: 113.7 MB (113676056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621eaefc355c8ff33315977f36c564b56529b9f878e8af23f138e95673d129e`  
		Last Modified: Tue, 04 Jul 2023 06:27:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5056202c38c8e3b88b20615d41c93fc958d6bf4a80bcc1a3b53765c232df6e3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.1 MB (151095312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd94729d9ee9304a370b1ba5ac646b8faaa650776487165626207b6276dbe975`
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
# Tue, 04 Jul 2023 03:53:42 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:01 GMT
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
	-	`sha256:41a4dc5dccca253e2aa8ac911ac7815d685a43fa9ed3a0ae94dbf2abaceaff29`  
		Last Modified: Tue, 04 Jul 2023 03:55:51 GMT  
		Size: 116.4 MB (116415969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc61605bab7c03fce76d6926e712aaefc9928e00025d64c796e4e222b5f7ab2`  
		Last Modified: Tue, 04 Jul 2023 03:55:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; 386

```console
$ docker pull julia@sha256:c03e763abd1ce1958730a814a20c7a1ce1435e64fef6695af23588eed2fc178f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156290528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e984d299c4a75d49225c3fbc5e3e291017be7fbb09b8f195ebbc6966fec38d94`
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
# Tue, 04 Jul 2023 08:53:53 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:17 GMT
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
	-	`sha256:efc2306d7bacc61b98692dfff1b673341c9e1fd92384e8ec9ef718fbfb73e54a`  
		Last Modified: Tue, 04 Jul 2023 08:56:44 GMT  
		Size: 120.3 MB (120294809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8544337e3567a9768a97fd7d17b05eab7360c12bdb92a9140524585c2fc14be4`  
		Last Modified: Tue, 04 Jul 2023 08:56:21 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine`

```console
$ docker pull julia@sha256:48212100c7b69a0a5ea68d7d375452ad169a85eafd87c740062e143597e6b95a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine` - linux; amd64

```console
$ docker pull julia@sha256:f9db4933a708ae86f0e89f04dfb77be6f48fec073b2e1bd548ff7e07755b927f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e8f8c6310b13b584db3297d92a85b05e756817dd55cea187a7f4b3c1c981d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:14:58 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b14b8c15ddbe32a9d67d670852149497149928cac8d6db33b30b70d28afdf0a`  
		Last Modified: Thu, 15 Jun 2023 00:17:43 GMT  
		Size: 121.8 MB (121829514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3972cf1468f8db4d4ba693b4511092b7c9e32fc1a6413bad0b1f7064da70d`  
		Last Modified: Thu, 15 Jun 2023 00:17:26 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.17`

```console
$ docker pull julia@sha256:92185c71acc5290d8dbc4d23deee54a3cd0ac8f2b51a32dc5261df9362615c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2df858e1d333ccf9a097e2b810600bf881651f8b5316a05dca5e62968fb4c299
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125204631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9242533c211a85926b20781d026374068fd209172cc69dcd40dfe497c8a0dce2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:15:19 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:31 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c1bec9354fb7c25c6a8f40a4568daf57e0f9a4a5c965036793baa6be8557fb`  
		Last Modified: Thu, 15 Jun 2023 00:18:13 GMT  
		Size: 121.8 MB (121829545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca91bfa84b37afae43457469b7b6ed30faf890c63620fcfb04007180d83f5e4e`  
		Last Modified: Thu, 15 Jun 2023 00:17:56 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.18`

```console
$ docker pull julia@sha256:48212100c7b69a0a5ea68d7d375452ad169a85eafd87c740062e143597e6b95a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:f9db4933a708ae86f0e89f04dfb77be6f48fec073b2e1bd548ff7e07755b927f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e8f8c6310b13b584db3297d92a85b05e756817dd55cea187a7f4b3c1c981d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 15 Jun 2023 00:14:58 GMT
ENV JULIA_VERSION=1.6.7
# Thu, 15 Jun 2023 00:15:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jun 2023 00:15:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:15:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:15:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b14b8c15ddbe32a9d67d670852149497149928cac8d6db33b30b70d28afdf0a`  
		Last Modified: Thu, 15 Jun 2023 00:17:43 GMT  
		Size: 121.8 MB (121829514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3972cf1468f8db4d4ba693b4511092b7c9e32fc1a6413bad0b1f7064da70d`  
		Last Modified: Thu, 15 Jun 2023 00:17:26 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-bookworm`

```console
$ docker pull julia@sha256:81290e372fb84a653b1ceb07a2e13f93af6dda3f5197191cde95ace5a08a5bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:e5e1d337433439da417b79ca51cd63698fc48e7ff032b6b1f1c46b3b808570c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157448493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff62465e425cd7947df6c2eaa5231b1395cef69314b3b07051e72b3395b7d1`
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
# Tue, 04 Jul 2023 12:57:46 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:01 GMT
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
	-	`sha256:3d5c0da1f8ee41aadc9bf9f49aef04ca0203aac6d219a9c528168488834e2ebd`  
		Last Modified: Tue, 04 Jul 2023 13:00:22 GMT  
		Size: 122.6 MB (122627479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26872efe14570e5349d5d332f0adeac8e1e17930860e3fc68ce81a03e9b8f9e9`  
		Last Modified: Tue, 04 Jul 2023 13:00:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bookworm` - linux; arm variant v7

```console
$ docker pull julia@sha256:2ab09c60ea80307493ca999611b6dbdcfd7fecdab736caf8dd973aadb0070a5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143294057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81ef026a69b9806a304414ff48ee16616123a66928838e8631c7095241ce4945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:26:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:26:33 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:26:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:26:59 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db77a978ab7f92a239b0408105fd78a65e1664b8e8ece6366e8a47461a506e24`  
		Last Modified: Tue, 04 Jul 2023 06:27:51 GMT  
		Size: 4.8 MB (4816363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43958bd99698dbd25abd055f5a29a7f2c249b36f8d595f7901ff169784cd6b9`  
		Last Modified: Tue, 04 Jul 2023 06:28:12 GMT  
		Size: 113.7 MB (113676056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621eaefc355c8ff33315977f36c564b56529b9f878e8af23f138e95673d129e`  
		Last Modified: Tue, 04 Jul 2023 06:27:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5056202c38c8e3b88b20615d41c93fc958d6bf4a80bcc1a3b53765c232df6e3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.1 MB (151095312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd94729d9ee9304a370b1ba5ac646b8faaa650776487165626207b6276dbe975`
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
# Tue, 04 Jul 2023 03:53:42 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:01 GMT
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
	-	`sha256:41a4dc5dccca253e2aa8ac911ac7815d685a43fa9ed3a0ae94dbf2abaceaff29`  
		Last Modified: Tue, 04 Jul 2023 03:55:51 GMT  
		Size: 116.4 MB (116415969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc61605bab7c03fce76d6926e712aaefc9928e00025d64c796e4e222b5f7ab2`  
		Last Modified: Tue, 04 Jul 2023 03:55:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bookworm` - linux; 386

```console
$ docker pull julia@sha256:c03e763abd1ce1958730a814a20c7a1ce1435e64fef6695af23588eed2fc178f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.3 MB (156290528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e984d299c4a75d49225c3fbc5e3e291017be7fbb09b8f195ebbc6966fec38d94`
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
# Tue, 04 Jul 2023 08:53:53 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:17 GMT
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
	-	`sha256:efc2306d7bacc61b98692dfff1b673341c9e1fd92384e8ec9ef718fbfb73e54a`  
		Last Modified: Tue, 04 Jul 2023 08:56:44 GMT  
		Size: 120.3 MB (120294809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8544337e3567a9768a97fd7d17b05eab7360c12bdb92a9140524585c2fc14be4`  
		Last Modified: Tue, 04 Jul 2023 08:56:21 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-bullseye`

```console
$ docker pull julia@sha256:bf24ff1eb752d5b837334acad7cd8c95718f6e976b8f115c9fa549eabc390a1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:2eaa299a228888695a12824ab8416a838ac14319f1f3fd53308946118de74b18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156484503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdea7ff13328a8e22bc36bdc348ad705b51930de3c3674ae90b4ce531cb131ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 12:58:05 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 12:58:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 12:58:21 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:58:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 12:58:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef54198d58cd5f9737d61a032200003a68a1eeabe41f38661bde18f23ccfac44`  
		Last Modified: Tue, 04 Jul 2023 13:00:48 GMT  
		Size: 122.6 MB (122640066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71befbca109de1b0e96c2ebd0bda47988c67bbdb2219eca79f27c3bed4d05def`  
		Last Modified: Tue, 04 Jul 2023 13:00:30 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:5507fc803951e5d7d6bc3ab131884db671da38de9b9e0ecbb8aff568bb2dd7b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142495992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415357620180759f54d516711f562be5b3583e8692074e914b4f16a1744d8c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:27:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:27:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 06:27:13 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 06:27:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 06:27:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:27:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:27:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7a9ee38b3bace42d79860e8d0f20a27ab6851a4c4d931a4fe5d7c513d6aea`  
		Last Modified: Tue, 04 Jul 2023 06:28:21 GMT  
		Size: 2.2 MB (2228939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16543aa34ebb99eee649999641723c251c7d3b571726b7c585e71fce686bbd4`  
		Last Modified: Tue, 04 Jul 2023 06:28:41 GMT  
		Size: 113.7 MB (113687926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb00013048d915815a9aae6a11e9969470bbea37f34b3ac2d165d89b55f1d6`  
		Last Modified: Tue, 04 Jul 2023 06:28:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1b45c09df9ae2097879d4eb1376a32a9fa70cfc3a7309d03e2c831c8d28126d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148906138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4078b7c4a11b4a16232f9835a35fc1b634a5264fb0b37cfc4286b364450829cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 03:54:05 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 03:54:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 03:54:21 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:54:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:54:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c6c16eb8611d5f73aaf1004452d08d9a59e6fed1f4c22e99fdb2d4ac17acd9`  
		Last Modified: Tue, 04 Jul 2023 03:56:12 GMT  
		Size: 116.4 MB (116428395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631d3696ceee8180e5f6de536e4482cf1982bd3116c4c61b4aea079df1d4494f`  
		Last Modified: Tue, 04 Jul 2023 03:55:59 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; 386

```console
$ docker pull julia@sha256:6ee273b3181c594cc0f03d355b6a75b4cf1ef10a188c411fce09a713f46cd6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155237947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad331954ef6fcbd49eb58fcabd8b718144e4c13efbb6c8cd4fffe3d8c5229cb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 04 Jul 2023 08:54:21 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 04 Jul 2023 08:54:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 04 Jul 2023 08:54:42 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 04 Jul 2023 08:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 08:54:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78c00973a02bf0768ad9012c721ff22e529b3ef7ed44a69cbf8b0de03866f22`  
		Last Modified: Tue, 04 Jul 2023 08:57:19 GMT  
		Size: 120.3 MB (120307546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ca4fd5e402f51c93f9c8ff5bc51da54aebdfafb3ef3d88bada6cebf1acad7`  
		Last Modified: Tue, 04 Jul 2023 08:56:55 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore`

```console
$ docker pull julia@sha256:9883f88d57cdcca134f39df309332d01684fee43969649dd5f6866877d651768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6.7-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-1809`

```console
$ docker pull julia@sha256:f069b3a89018b1362a9b10b945fd96a2a8bf830ab182606fa766fbb8b45cc81e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:1.6.7-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:17bf2b233176abd0241026d146cdda71267c345270affe73c4870d5fa25a14dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1785100354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011fbde06967e9fe5463654a7f843fb372d1b098fa0ada7786b6284b8ef27b9c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:48:15 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:48:16 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:48:17 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:49:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:49:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a92393738de647804f7da1baa0739fe569d88962b59b230493fa4daa6f134`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e8200691b4af474594da4fb1e426208a63dccb91014f097f2b13a6b47c42b`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033ab7cf1bd3235ee357cd1042633037f8723c48ab5f419d47818b56570821f`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bf3774435f91302835d4e8c53a8fb0a39d50ed0ae29ad01a786a0381505e42`  
		Last Modified: Sat, 24 Jun 2023 03:52:44 GMT  
		Size: 134.4 MB (134356488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57c9278f4211def6f06d84de5425fb46091b829d1e695d41c3e59f4fda06d8`  
		Last Modified: Sat, 24 Jun 2023 03:52:18 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:a72a9850d0f754213d8fa95591301d2217a4ea33799489b4cb4be82a2998ceb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:1.6.7-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:f91a935da240eaa45f7242c7f8f6bbeb8c050c90b0cd5bea2c2813cd673143eb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560673312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc5d9de13937c08a840ca69b6cdd98ef2dc1a46932cfbb057e4af92cd1865d7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:46:46 GMT
ENV JULIA_VERSION=1.6.7
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Sat, 24 Jun 2023 03:46:47 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Sat, 24 Jun 2023 03:47:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 24 Jun 2023 03:48:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e206be00e70624f4ba69004b9a0976381a8c9e52ce619de77743a39203e`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5644bdcebb00609680e0d8e7cd9da716a3ab0874ca841bd6591b809da8d26`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4bfedfd80bb3948e3d0156d36c6fd934ccb1cfece8cde25b961fcea07d6a8a`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d301d5e0254946ca533cad379602ed7acf25b5dab7372b11f1bd78047e0370`  
		Last Modified: Sat, 24 Jun 2023 03:52:09 GMT  
		Size: 134.4 MB (134367608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e645dd601e3964c5eff93fe5b73eb731a6bf82dd2062407cac82629f75e68`  
		Last Modified: Sat, 24 Jun 2023 03:51:41 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9`

```console
$ docker pull julia@sha256:e95993d17016c2df34d63bc7d2a0673e69f92d06cb1e393f0217894a874a8b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine3.17`

```console
$ docker pull julia@sha256:d5c4035b68e660e213772c08e46a9efb70895aa397f664dda89344cf1b066bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2e3b7d449f63f6759404bf3e414164559d8b56d076ae10a7d9493b153dccefca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154517691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fecf32bc21e8f19277b73f5ae1fbfbb7f61996eec72e6db0b3c341c0d83c35f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:25:01 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:25:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:25:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:25:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aca3cbabb864e81b14b1cf75dee6cb4a5c034a5c4d529b4dd548c708ad7585`  
		Last Modified: Thu, 06 Jul 2023 20:28:15 GMT  
		Size: 151.1 MB (151142605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5584a8659f45d6418de9bea871a53ad36743c215f9cdcc65b2bf41c93df8f8eb`  
		Last Modified: Thu, 06 Jul 2023 20:27:53 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine3.18`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-bookworm`

```console
$ docker pull julia@sha256:9a8f501b64033b3267f3e20254b9dd760c27c41b3df74dbc78f65c7a3eb92769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bookworm` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-bullseye`

```console
$ docker pull julia@sha256:b8c7552ed06d657777a1cbe5d0b8e3612f50c5b5fa481a86c8eb97fb46e0e75c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:aaeaaa3d7dbaef6d2ec4cc5a7411ec9a9c0c69b174af53cdc0cdf3c35b7cf7b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182827655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8faa5f3694dc11c54608231a241f0e22b0ab343df1cf658181ccb08fa52feea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:38 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5ba2316d48362d9eb272a6551eafd1093f623c54f771aa94b0505319d83801`  
		Last Modified: Thu, 06 Jul 2023 20:26:56 GMT  
		Size: 149.0 MB (148983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbbc851898f4fe7e45d809b9c5b6e29ae7775d8e4da389a76824adb60cfecf4`  
		Last Modified: Thu, 06 Jul 2023 20:26:34 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:421f13803f4850ea52d09920f12147c018596841b7009a896bf6ad35c358bd5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175594642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a550b8c8f1775b3a11fad42cae90fe5af0c2d6e92b0cbd293277cbe54a7af289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:54:08 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:54:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb4f341423d35b379731ed8751938166da78d0156cc03ee3e5ac5c50215add`  
		Last Modified: Thu, 06 Jul 2023 19:55:35 GMT  
		Size: 143.1 MB (143116901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae40477f57ed335e0bcea787cfc74221033f2504aef4c8e2c7f9979ee3f367`  
		Last Modified: Thu, 06 Jul 2023 19:55:18 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ce5938fb6fe97c2bc0f89fec3e1137d9e577b5d1689fc20308a6cbe4dca01d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172541142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7162832f8861471c6e00bc1df0a84f210b183eeae363bb5568d685e476e30b04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:41:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:44 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb637a0e859dfa93ee87c91ea9411f73f8f3ac5b7dcf5cd93df78c651f0fcba4`  
		Last Modified: Thu, 06 Jul 2023 19:43:16 GMT  
		Size: 137.6 MB (137610741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee123d90de401331f01e2bfcde57c1b8f99c35ae344edf4da35365cfd22eaf`  
		Last Modified: Thu, 06 Jul 2023 19:42:48 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:41c46f675bfea61c7cfa392e0ae5e62e86121a60e929048ce44383fd3a305b2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171241827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97355cbc9364a46b4490c47295e6169f0825bc3c623e868573f56c96f9862aa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:33 GMT
ADD file:37fa020aca7253d41d395ed529c38db73caaa4da098754836244552f65fa7d5d in / 
# Tue, 04 Jul 2023 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:42:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:42:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:42:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:42:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:17:48 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:18:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:18:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:18:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:147bb8b5828c99cd6b07d252d2987490463c142099eaa0815025685f8fa4f3d8`  
		Last Modified: Tue, 04 Jul 2023 01:25:40 GMT  
		Size: 35.3 MB (35291082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6ddbab4eda0628b3aa67cecb27fb39624b779814fe84d9f47de75724b8f22f`  
		Last Modified: Tue, 04 Jul 2023 06:44:40 GMT  
		Size: 2.6 MB (2627602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78898475b67599608955aad6821eaf3eea34dbb639469120507a4eac042c28`  
		Last Modified: Thu, 06 Jul 2023 20:20:34 GMT  
		Size: 133.3 MB (133322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45330019a76b147b8f737bb6f568c7828a1120f0aa94bd6c0d244df64d36dba0`  
		Last Modified: Thu, 06 Jul 2023 20:19:58 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore`

```console
$ docker pull julia@sha256:81c6d8b118fd0fab2967dc9187bc3c31a5d6e016197563adacf1c0aa1a634078
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore-1809`

```console
$ docker pull julia@sha256:c72611e6cce79bcf49a5cd17fe3caeecfab0852fee938a219ef20302f8b5c0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:e4fc96d43a5cead4e8df2c841d75020c9d9b7b6f2e680e981b531ff190a47559
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:1.9-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2`

```console
$ docker pull julia@sha256:e95993d17016c2df34d63bc7d2a0673e69f92d06cb1e393f0217894a874a8b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9.2` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-alpine`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.2-alpine` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-alpine3.17`

```console
$ docker pull julia@sha256:d5c4035b68e660e213772c08e46a9efb70895aa397f664dda89344cf1b066bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.2-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2e3b7d449f63f6759404bf3e414164559d8b56d076ae10a7d9493b153dccefca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154517691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fecf32bc21e8f19277b73f5ae1fbfbb7f61996eec72e6db0b3c341c0d83c35f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:25:01 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:25:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:25:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:25:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aca3cbabb864e81b14b1cf75dee6cb4a5c034a5c4d529b4dd548c708ad7585`  
		Last Modified: Thu, 06 Jul 2023 20:28:15 GMT  
		Size: 151.1 MB (151142605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5584a8659f45d6418de9bea871a53ad36743c215f9cdcc65b2bf41c93df8f8eb`  
		Last Modified: Thu, 06 Jul 2023 20:27:53 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-alpine3.18`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.2-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-bookworm`

```console
$ docker pull julia@sha256:9a8f501b64033b3267f3e20254b9dd760c27c41b3df74dbc78f65c7a3eb92769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9.2-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bookworm` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-bullseye`

```console
$ docker pull julia@sha256:b8c7552ed06d657777a1cbe5d0b8e3612f50c5b5fa481a86c8eb97fb46e0e75c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9.2-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:aaeaaa3d7dbaef6d2ec4cc5a7411ec9a9c0c69b174af53cdc0cdf3c35b7cf7b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182827655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8faa5f3694dc11c54608231a241f0e22b0ab343df1cf658181ccb08fa52feea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:38 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5ba2316d48362d9eb272a6551eafd1093f623c54f771aa94b0505319d83801`  
		Last Modified: Thu, 06 Jul 2023 20:26:56 GMT  
		Size: 149.0 MB (148983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbbc851898f4fe7e45d809b9c5b6e29ae7775d8e4da389a76824adb60cfecf4`  
		Last Modified: Thu, 06 Jul 2023 20:26:34 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:421f13803f4850ea52d09920f12147c018596841b7009a896bf6ad35c358bd5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175594642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a550b8c8f1775b3a11fad42cae90fe5af0c2d6e92b0cbd293277cbe54a7af289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:54:08 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:54:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb4f341423d35b379731ed8751938166da78d0156cc03ee3e5ac5c50215add`  
		Last Modified: Thu, 06 Jul 2023 19:55:35 GMT  
		Size: 143.1 MB (143116901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae40477f57ed335e0bcea787cfc74221033f2504aef4c8e2c7f9979ee3f367`  
		Last Modified: Thu, 06 Jul 2023 19:55:18 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bullseye` - linux; 386

```console
$ docker pull julia@sha256:ce5938fb6fe97c2bc0f89fec3e1137d9e577b5d1689fc20308a6cbe4dca01d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172541142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7162832f8861471c6e00bc1df0a84f210b183eeae363bb5568d685e476e30b04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:41:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:44 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb637a0e859dfa93ee87c91ea9411f73f8f3ac5b7dcf5cd93df78c651f0fcba4`  
		Last Modified: Thu, 06 Jul 2023 19:43:16 GMT  
		Size: 137.6 MB (137610741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee123d90de401331f01e2bfcde57c1b8f99c35ae344edf4da35365cfd22eaf`  
		Last Modified: Thu, 06 Jul 2023 19:42:48 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:41c46f675bfea61c7cfa392e0ae5e62e86121a60e929048ce44383fd3a305b2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171241827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97355cbc9364a46b4490c47295e6169f0825bc3c623e868573f56c96f9862aa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:33 GMT
ADD file:37fa020aca7253d41d395ed529c38db73caaa4da098754836244552f65fa7d5d in / 
# Tue, 04 Jul 2023 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:42:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:42:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:42:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:42:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:17:48 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:18:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:18:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:18:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:147bb8b5828c99cd6b07d252d2987490463c142099eaa0815025685f8fa4f3d8`  
		Last Modified: Tue, 04 Jul 2023 01:25:40 GMT  
		Size: 35.3 MB (35291082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6ddbab4eda0628b3aa67cecb27fb39624b779814fe84d9f47de75724b8f22f`  
		Last Modified: Tue, 04 Jul 2023 06:44:40 GMT  
		Size: 2.6 MB (2627602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78898475b67599608955aad6821eaf3eea34dbb639469120507a4eac042c28`  
		Last Modified: Thu, 06 Jul 2023 20:20:34 GMT  
		Size: 133.3 MB (133322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45330019a76b147b8f737bb6f568c7828a1120f0aa94bd6c0d244df64d36dba0`  
		Last Modified: Thu, 06 Jul 2023 20:19:58 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-windowsservercore`

```console
$ docker pull julia@sha256:81c6d8b118fd0fab2967dc9187bc3c31a5d6e016197563adacf1c0aa1a634078
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9.2-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.2-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-windowsservercore-1809`

```console
$ docker pull julia@sha256:c72611e6cce79bcf49a5cd17fe3caeecfab0852fee938a219ef20302f8b5c0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:1.9.2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.2-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:e4fc96d43a5cead4e8df2c841d75020c9d9b7b6f2e680e981b531ff190a47559
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:1.9.2-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.17`

```console
$ docker pull julia@sha256:d5c4035b68e660e213772c08e46a9efb70895aa397f664dda89344cf1b066bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2e3b7d449f63f6759404bf3e414164559d8b56d076ae10a7d9493b153dccefca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154517691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fecf32bc21e8f19277b73f5ae1fbfbb7f61996eec72e6db0b3c341c0d83c35f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:25:01 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:25:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:25:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:25:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aca3cbabb864e81b14b1cf75dee6cb4a5c034a5c4d529b4dd548c708ad7585`  
		Last Modified: Thu, 06 Jul 2023 20:28:15 GMT  
		Size: 151.1 MB (151142605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5584a8659f45d6418de9bea871a53ad36743c215f9cdcc65b2bf41c93df8f8eb`  
		Last Modified: Thu, 06 Jul 2023 20:27:53 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.18`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:bookworm`

```console
$ docker pull julia@sha256:9a8f501b64033b3267f3e20254b9dd760c27c41b3df74dbc78f65c7a3eb92769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:bookworm` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:bullseye`

```console
$ docker pull julia@sha256:b8c7552ed06d657777a1cbe5d0b8e3612f50c5b5fa481a86c8eb97fb46e0e75c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:aaeaaa3d7dbaef6d2ec4cc5a7411ec9a9c0c69b174af53cdc0cdf3c35b7cf7b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182827655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8faa5f3694dc11c54608231a241f0e22b0ab343df1cf658181ccb08fa52feea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 12:57:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 12:57:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:38 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abcd95f4328c01db67acd78a60986f520af8f08f5578354556536746d96c8c`  
		Last Modified: Tue, 04 Jul 2023 12:59:27 GMT  
		Size: 2.4 MB (2426676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5ba2316d48362d9eb272a6551eafd1093f623c54f771aa94b0505319d83801`  
		Last Modified: Thu, 06 Jul 2023 20:26:56 GMT  
		Size: 149.0 MB (148983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbbc851898f4fe7e45d809b9c5b6e29ae7775d8e4da389a76824adb60cfecf4`  
		Last Modified: Thu, 06 Jul 2023 20:26:34 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:421f13803f4850ea52d09920f12147c018596841b7009a896bf6ad35c358bd5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175594642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a550b8c8f1775b3a11fad42cae90fe5af0c2d6e92b0cbd293277cbe54a7af289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 03:53:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 03:53:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:54:08 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:54:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260593f69f95c4991d15c272363825d569810fa8bf90aea493bbae373d3c80c`  
		Last Modified: Tue, 04 Jul 2023 03:55:07 GMT  
		Size: 2.4 MB (2414414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb4f341423d35b379731ed8751938166da78d0156cc03ee3e5ac5c50215add`  
		Last Modified: Thu, 06 Jul 2023 19:55:35 GMT  
		Size: 143.1 MB (143116901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bae40477f57ed335e0bcea787cfc74221033f2504aef4c8e2c7f9979ee3f367`  
		Last Modified: Thu, 06 Jul 2023 19:55:18 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:ce5938fb6fe97c2bc0f89fec3e1137d9e577b5d1689fc20308a6cbe4dca01d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172541142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7162832f8861471c6e00bc1df0a84f210b183eeae363bb5568d685e476e30b04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 08:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 08:53:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 08:53:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 19:41:17 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:44 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a09ccc50da5179fdb6f531f0063c679f167520c0d141195aafaecf53391cf`  
		Last Modified: Tue, 04 Jul 2023 08:55:40 GMT  
		Size: 2.5 MB (2532534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb637a0e859dfa93ee87c91ea9411f73f8f3ac5b7dcf5cd93df78c651f0fcba4`  
		Last Modified: Thu, 06 Jul 2023 19:43:16 GMT  
		Size: 137.6 MB (137610741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee123d90de401331f01e2bfcde57c1b8f99c35ae344edf4da35365cfd22eaf`  
		Last Modified: Thu, 06 Jul 2023 19:42:48 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:41c46f675bfea61c7cfa392e0ae5e62e86121a60e929048ce44383fd3a305b2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171241827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97355cbc9364a46b4490c47295e6169f0825bc3c623e868573f56c96f9862aa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:33 GMT
ADD file:37fa020aca7253d41d395ed529c38db73caaa4da098754836244552f65fa7d5d in / 
# Tue, 04 Jul 2023 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:42:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:42:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 04 Jul 2023 06:42:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 06:42:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:17:48 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:18:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:18:37 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:18:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:147bb8b5828c99cd6b07d252d2987490463c142099eaa0815025685f8fa4f3d8`  
		Last Modified: Tue, 04 Jul 2023 01:25:40 GMT  
		Size: 35.3 MB (35291082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6ddbab4eda0628b3aa67cecb27fb39624b779814fe84d9f47de75724b8f22f`  
		Last Modified: Tue, 04 Jul 2023 06:44:40 GMT  
		Size: 2.6 MB (2627602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78898475b67599608955aad6821eaf3eea34dbb639469120507a4eac042c28`  
		Last Modified: Thu, 06 Jul 2023 20:20:34 GMT  
		Size: 133.3 MB (133322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45330019a76b147b8f737bb6f568c7828a1120f0aa94bd6c0d244df64d36dba0`  
		Last Modified: Thu, 06 Jul 2023 20:19:58 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:e95993d17016c2df34d63bc7d2a0673e69f92d06cb1e393f0217894a874a8b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:79d2fdde57b837b6627ee55690d2bd4ca9ec72bd5f75110fa0b5a1d8601e4112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1cbbf3f27215b4b5a64b3a0ca20c954fa0225a27c8fe3cac7184802cb3d16b`
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
# Thu, 06 Jul 2023 20:23:53 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:24:13 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:14 GMT
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
	-	`sha256:86dddcf3e65ce5f4a2d3ff8d86f01cc008c5cfdbdf2dae32428238149e590548`  
		Last Modified: Thu, 06 Jul 2023 20:26:22 GMT  
		Size: 149.0 MB (148971271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cfdb150b09385f4ac058c587bf88a11e7c4d0f407461b5398facfbfef666aa`  
		Last Modified: Thu, 06 Jul 2023 20:25:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ca40e951551c22489a35a2d5962b89dc422d82d0830e2f5dd4db8943c8c306e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177783168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae963f844ec6e52639af22136e49b3fbc3c1c894a181850ca4d9147e962b27f`
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
# Thu, 06 Jul 2023 19:53:40 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:53:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:54:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:54:02 GMT
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
	-	`sha256:6f10a2c5c03b34dc470462238272266d79fe0f4dc9f5d607db01d10f47ed62a2`  
		Last Modified: Thu, 06 Jul 2023 19:55:06 GMT  
		Size: 143.1 MB (143103825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabe1ed291cda4ff626a3d610b4da8e0bec7ab0e730db57c314407612fea19ea`  
		Last Modified: Thu, 06 Jul 2023 19:54:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:7e5741c6cc342e47aac838b5e889936a058a001962c503c6e5ff6426fa17d6ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173593600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342c0828044836d398d4d5b7c948ff2d0f6a36414ecc1655896ca300c8b9ccf4`
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
# Thu, 06 Jul 2023 19:40:37 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 19:41:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 19:41:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 19:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 19:41:11 GMT
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
	-	`sha256:9872d33bc90a88778d6df9c8e54593bc53c8ee28e55ae54640bf6121e85c57a9`  
		Last Modified: Thu, 06 Jul 2023 19:42:36 GMT  
		Size: 137.6 MB (137597876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fe97071015a4b43527c44e1c8df4892ba503e1732e222459bc911b47340ab`  
		Last Modified: Thu, 06 Jul 2023 19:42:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:120b7351823cb8fbf95bd535b07cf5ae3cdfe1de9b15acdf78953790c8bb934f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172657569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc66256695820bc102ee719a2d37f6792bec0600ad7825df5e20253c671e54f`
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
# Thu, 06 Jul 2023 20:16:49 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 06 Jul 2023 20:17:43 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:17:44 GMT
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
	-	`sha256:2be6880108159a689ff467b573c554c530480a04849107681093fa706198248d`  
		Last Modified: Thu, 06 Jul 2023 20:19:40 GMT  
		Size: 133.3 MB (133310591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5059e890d52bac0dfdc7c509bd62d29dbb33b601a641edf46ce672dd954cb81`  
		Last Modified: Thu, 06 Jul 2023 20:19:04 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore`

```console
$ docker pull julia@sha256:81c6d8b118fd0fab2967dc9187bc3c31a5d6e016197563adacf1c0aa1a634078
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `julia:windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:c72611e6cce79bcf49a5cd17fe3caeecfab0852fee938a219ef20302f8b5c0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:e4fc96d43a5cead4e8df2c841d75020c9d9b7b6f2e680e981b531ff190a47559
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull julia@sha256:09a9e3def5a2020304c146a707437628eb4dddfa645b3ad282ebc5b9518c3005
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587738412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad89dc1d5172e965645a3087841d68a8a8495bd8a34317b7d442a735bcb3dfe`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:23:02 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:23:03 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:24:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:24:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1b6e35fa467ad607882b47cd8429ff579147602d247ce19977b8bce5838f04`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1305a1895721deee857cf830a6cd9331bd73c6e45bd0d0ccaf330ba562a942df`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2798876dfa3b4a36180278f353399a66773dff25d20591b0f8b030b2e29382c5`  
		Last Modified: Thu, 06 Jul 2023 20:26:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad02a9b191e1c1addfe15a744974526845f08fa701c270fe5b100ce3b1eb5e9`  
		Last Modified: Thu, 06 Jul 2023 20:27:18 GMT  
		Size: 161.4 MB (161432706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4130011a81c46f206889ab332f20368c125ebde391bdb833d30d7b9bfd714959`  
		Last Modified: Thu, 06 Jul 2023 20:26:46 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
