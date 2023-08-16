## `julia:bookworm`

```console
$ docker pull julia@sha256:4175ba693fabc8ca1c92934395b95f5e029570d8b19c83912f757b5353b3d513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:bookworm` - linux; amd64

```console
$ docker pull julia@sha256:a4fcabe48a8f49b987deaeb888b4be6bfa50d5e5627467e1fa6886af069b4959
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183792191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746140f2a102eb0da4543cbb0ea5d9ec16f6efc919cba1180e13be657ef0b799`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:57:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:57:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:57:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:57:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 09:58:30 GMT
ENV JULIA_VERSION=1.9.2
# Wed, 16 Aug 2023 09:58:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 09:58:48 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 09:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 09:58:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8721124fc215962745673ef73dc19e3e00368bee1b4da37bc61b6832d5c29735`  
		Last Modified: Wed, 16 Aug 2023 10:00:40 GMT  
		Size: 5.7 MB (5695794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646f3294aa8c4aa25e3bb74950ed889329782fc380a5694b49e344b1facbb715`  
		Last Modified: Wed, 16 Aug 2023 10:02:16 GMT  
		Size: 149.0 MB (148971462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5f5dac457adbbeaedb336cb8497f024160534e678b1222081105bc3f669484`  
		Last Modified: Wed, 16 Aug 2023 10:01:54 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b5257c4647bbd64715d2b4902a0ea8aacf071f73e7b2013bfdf2d8ce3f8024cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177788571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372bb7d51e93e36789159b5d18961a39ee474ccc2e977cc379ef06c72a74cf9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:29:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:29:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:29:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:29:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 03:30:28 GMT
ENV JULIA_VERSION=1.9.2
# Wed, 16 Aug 2023 03:30:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 03:30:51 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:30:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 03:30:51 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9ec7a2dd557caa143329ea7f6b0082a7529fe353e771325fc91731ef6a525`  
		Last Modified: Wed, 16 Aug 2023 03:32:10 GMT  
		Size: 5.5 MB (5527026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856bc39800a7015b5f0bad41e1f68c4d72ab3f96244e89fa8909cb8169bf1542`  
		Last Modified: Wed, 16 Aug 2023 03:33:24 GMT  
		Size: 143.1 MB (143103914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ef1227929903dfba2e690a3c3c8e280fd3169437bab4cb6f6f44c5ed1cc559`  
		Last Modified: Wed, 16 Aug 2023 03:33:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; 386

```console
$ docker pull julia@sha256:82a04feb0c19dc43b03e18c65fc4293eb8a0db0f59b6fb28fbbffc87d389a6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173594749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ee61405792ed83d8f1d33e54f90c1b5b598c6ddf94a3fbdce550d46f2bc8e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:28:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:28:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:28:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:28:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 09:29:59 GMT
ENV JULIA_VERSION=1.9.2
# Wed, 16 Aug 2023 09:30:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 09:30:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 09:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 09:30:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45508e354104caec85eedf213ac7fda6a301c8b3dcc8f54624f48dc743b73d`  
		Last Modified: Wed, 16 Aug 2023 09:32:17 GMT  
		Size: 5.9 MB (5854584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6446e25f285540fc40017ebb1f02410ce840dcfc9a4f2f3bf27e6ef169079772`  
		Last Modified: Wed, 16 Aug 2023 09:34:08 GMT  
		Size: 137.6 MB (137597967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70752332b1efb5e3b3aafe0becf80505ed3a4c7a88ad704c90bf57a3a4492ab2`  
		Last Modified: Wed, 16 Aug 2023 09:33:39 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:99550af6fe37fb9e4f748277dbfdba60f0ce49ad79de228586e0eed517eb0d9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172660157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:521e3e6027e7f0529529a4a91a179ea3f29864964075cadc7dd145e0111f92d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:33 GMT
ADD file:9578bf6d6b33f2ba960ab9309642d1c9dcc131d7b9e6f818b8cc4b843fe3aec8 in / 
# Wed, 16 Aug 2023 01:09:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:47:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:48:00 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:48:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 03:51:00 GMT
ENV JULIA_VERSION=1.9.2
# Wed, 16 Aug 2023 03:51:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz'; 			sha256='4c2d799f442d7fe718827b19da2bacb72ea041b9ce55f24eee7b1313f57c4383'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.2-linux-aarch64.tar.gz'; 			sha256='682397f8895149f0e283f0b27bffc6694033bdfb19f9366c80f6efdf3685f27c'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.2-linux-i686.tar.gz'; 			sha256='08d1f72d92772c9a1074196a4651e06ccadc290d6d1e316fb25a43e585c14db9'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.2-linux-ppc64le.tar.gz'; 			sha256='b03080f0f8aeff395de932b90716cc71cf93b6fd21c993e87bf0f6cfef25510d'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 03:51:58 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 03:51:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0500920b409f06d69819525676ebf090702285435050f7b1f973c8c7b034ea7c`  
		Last Modified: Wed, 16 Aug 2023 01:15:59 GMT  
		Size: 33.1 MB (33119300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f30a0c06039c467cf0e1b6990bc9fe73f6347c0a9a3762abb5def24e2e8086b`  
		Last Modified: Wed, 16 Aug 2023 03:53:55 GMT  
		Size: 6.2 MB (6229794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d097109c721dcbfae72939bac1bb3cb572426ab6d6e78d472a3e748d55f2d7`  
		Last Modified: Wed, 16 Aug 2023 03:56:17 GMT  
		Size: 133.3 MB (133310687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c1a95cb63db8d023eb8f41bfe5ce8f0564c35667651ed15a544c8a3e75fdf`  
		Last Modified: Wed, 16 Aug 2023 03:55:41 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
