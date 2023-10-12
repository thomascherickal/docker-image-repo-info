## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:b41edc63d5a464ca0a0d10aa150e7f1b0b0490421feb579da1a95dba9cd09ac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:63e334a6dc1052f88fead0df38f694ef323f0c847d6d33e4ba087d9d1bbb4f98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203899876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce56529dddc8eb8db503464ce08ef7982737edbbdda0dba14aa73fd9b63719f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:27:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 Oct 2023 20:27:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:27:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 Oct 2023 20:27:25 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Wed, 11 Oct 2023 20:27:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 Oct 2023 20:27:46 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:27:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Oct 2023 20:27:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa7011b05f9e29ea30be6216296e0b6d82aac57d46028dad60c3beddb691310`  
		Last Modified: Wed, 11 Oct 2023 20:30:56 GMT  
		Size: 2.4 MB (2427566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01629ad5fb0f3c083dc1ddfd6c7fdaf626060742b774db946ee0b4bf4a15039`  
		Last Modified: Wed, 11 Oct 2023 20:31:20 GMT  
		Size: 170.1 MB (170054074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2dee088dcdf196792560e458c226274763000cee0ea9abf8eda62304337e701`  
		Last Modified: Wed, 11 Oct 2023 20:30:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:b22db381235c89f97d59e97ca7ee734ec0165dcef7a206c6cbd7f52ba12e70a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197232471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794c25dad085fd11c1abf35a102eb42466db679f4527d5aaa624b85e2c5b4e3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:12:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 12 Oct 2023 10:12:07 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 10:12:07 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 12 Oct 2023 10:12:08 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Thu, 12 Oct 2023 10:12:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 12 Oct 2023 10:12:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 12 Oct 2023 10:12:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 10:12:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b77703c3351bcd6aa1cdd0536734a4bb7b0409c797c02f6cc36a70ee5f9450`  
		Last Modified: Thu, 12 Oct 2023 10:14:56 GMT  
		Size: 2.4 MB (2417361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f3e7dd26a64b04294cbfc88095c80f6d6bc6df104556f65935568cfe4d4661`  
		Last Modified: Thu, 12 Oct 2023 10:15:15 GMT  
		Size: 164.8 MB (164750651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0624d0a7e7c6a6be8969284fb8f9fddec34544bd64f9d2a75fb8ffea622209`  
		Last Modified: Thu, 12 Oct 2023 10:14:55 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:219d9dc90a6ef283827843f1231bf9d76e8d0c4e6e7c9f6f79533e6263797103
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191661161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511f38a6b685eb809a7d78b183691284623ca15407d75e32fe96807b028a1c81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:48:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:48:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 Oct 2023 21:48:18 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 21:48:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 Oct 2023 21:48:19 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Wed, 11 Oct 2023 21:48:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 Oct 2023 21:48:46 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:48:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:48:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e021d4becbac62cace4eb6bc7b7a731f7afc91f6d5fb2f13951e144aea7f4af6`  
		Last Modified: Wed, 11 Oct 2023 21:52:02 GMT  
		Size: 2.5 MB (2534874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8924a708c17b651c4897d9cd62a24968de5f1f3b4144d84774934665c9f78e`  
		Last Modified: Wed, 11 Oct 2023 21:52:34 GMT  
		Size: 156.7 MB (156723263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fd300cdb10f6241d126a0fe20a1a1b860381e75a851d4dcb86e44b64fe785d`  
		Last Modified: Wed, 11 Oct 2023 21:52:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:11aff9df2198408ad50a304fbadd4d182e71df2e6451e8ff3b146391da2903c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191974317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3a993b7827bd7a2328ed73c4f9f5e87701f5e77e7610d4734ad5bf1e60713a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:46:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:46:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 Oct 2023 20:46:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:46:08 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 Oct 2023 20:46:08 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Wed, 11 Oct 2023 20:46:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 Oct 2023 20:47:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Oct 2023 20:47:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21481d63f086cd73c034e7d64504abfab258026208d27e4f0390f32a2cfa81f`  
		Last Modified: Wed, 11 Oct 2023 20:50:33 GMT  
		Size: 2.6 MB (2631677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eecd4e480eb7fd40b7652f25d79b4a61b4dccda0e63c67f021483a0b330f946`  
		Last Modified: Wed, 11 Oct 2023 20:51:13 GMT  
		Size: 154.0 MB (154048551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8438c616762d218b8e882a564d499665c51621e6f3979dd5245bf561d91fd0d4`  
		Last Modified: Wed, 11 Oct 2023 20:50:32 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
