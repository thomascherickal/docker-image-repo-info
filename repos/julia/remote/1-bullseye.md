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
