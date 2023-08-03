## `julia:rc-bookworm`

```console
$ docker pull julia@sha256:8e0ab3648db01c9a02a4ba6b149445c30cccb42fd33fe2c68435709e7d85a71a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:98441976b343ed0fbb2b0224054720b7bbb12326cb0426045b9848875387d988
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208909773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089dbf4493532d493178a3d93202a1091a3dbc6a870b49032c1774f0cf9f5acf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:56:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 28 Jul 2023 01:56:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 01:56:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 28 Jul 2023 01:56:36 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Fri, 28 Jul 2023 01:56:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 28 Jul 2023 01:57:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:57:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f396ccff59167002913d510490ff01699857b722ce2c9f5d8f8fcfabf81dae47`  
		Last Modified: Fri, 28 Jul 2023 01:59:49 GMT  
		Size: 5.7 MB (5695805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf7fc7252500ce029c10ce4ec8f13b781a52717bcdbccbbd278eb19d9f624bf`  
		Last Modified: Fri, 28 Jul 2023 02:00:13 GMT  
		Size: 174.1 MB (174089063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68119a76085b84d7ab237267093966d2f15545ecc640d3bc94fc44523c2fa7ac`  
		Last Modified: Fri, 28 Jul 2023 01:59:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:35b603f2d6ab1aec49769ab42e185b5c7149dbe6b6cd35d10a66ebdc8b4738c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196279117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a74b21146173496133fb3ae4f06d972c3df45868ba21624df582ae938cd2b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:19:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 14:19:30 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 28 Jul 2023 14:19:30 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:19:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 02 Aug 2023 23:39:36 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 02 Aug 2023 23:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 02 Aug 2023 23:39:58 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 02 Aug 2023 23:39:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:39:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278c2a1c4be8ffa0998bbf3ae420ba10b300563d60d44af776c0fbb784be9af`  
		Last Modified: Fri, 28 Jul 2023 14:22:24 GMT  
		Size: 5.5 MB (5527018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9e7e41c59a368515e3e0b54700640b8165993ebeda94e44493f1c81e90841c`  
		Last Modified: Wed, 02 Aug 2023 23:41:10 GMT  
		Size: 161.6 MB (161594497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f607f6fd1b8d5f5477136826c0438e5894340c8eaa759caca45d444eddad5ee`  
		Last Modified: Wed, 02 Aug 2023 23:40:51 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; 386

```console
$ docker pull julia@sha256:f38a7655b313b18edc246f63d4d2be9a9e3172a0f86a624502268561165886a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.8 MB (189806912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749d2881a1330d9ff095be7b69945b0a7ed9bf17c40c1a945dad62a453ae0c66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:04:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 28 Jul 2023 00:04:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 00:04:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 02 Aug 2023 23:38:23 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 02 Aug 2023 23:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 02 Aug 2023 23:38:50 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 02 Aug 2023 23:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017b4dcfaea553337f724c97907de2678e47ea038b04e4dc006657aa31212b37`  
		Last Modified: Fri, 28 Jul 2023 00:08:26 GMT  
		Size: 5.9 MB (5854644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b055bb245d694b32071f9fe7cfa6ebf203ab999714956ccb9fe8a3704250838e`  
		Last Modified: Wed, 02 Aug 2023 23:40:25 GMT  
		Size: 153.8 MB (153810105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe36fde1489c115371dde3d9ec30f5ed82c5125e452da1877547ae8efedf1fb`  
		Last Modified: Wed, 02 Aug 2023 23:39:55 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:8c31bf1301659b7009228e38edc215e39d52c49d73681f645ac89fac43eaae6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197893180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1928885565019ede7314f107060706e3a2bf6cfba628de869a52d8544de6aa6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 07:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 07:44:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 28 Jul 2023 07:44:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 07:44:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 28 Jul 2023 07:44:54 GMT
ENV JULIA_VERSION=1.10.0-alpha1
# Fri, 28 Jul 2023 07:45:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-alpha1-linux-x86_64.tar.gz'; 			sha256='9aea120b126e54bf87a5bfcddc1c58d282272f6c7e3534f29e210a3c80290cfd'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-alpha1-linux-aarch64.tar.gz'; 			sha256='f56b5fb976621fbc5cdd98fb26c5bcfd94d21997ed0b36f9306b94e62f5e41fa'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-alpha1-linux-i686.tar.gz'; 			sha256='a37e4d5cae9ee39c30dddb3f5beb595c1e93de96867d88d5e1d017b91dfe924f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-alpha1-linux-ppc64le.tar.gz'; 			sha256='6c9ff07b56b847af530e7d2274956e0105765e03cfad4af3d3a7a8a00e17d2e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 28 Jul 2023 07:45:54 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 28 Jul 2023 07:45:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 07:45:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5286e7e75f66a0ad1e7bc0459a512c23758ac72ec1c96f0ed2b6842e924358c2`  
		Last Modified: Fri, 28 Jul 2023 07:49:49 GMT  
		Size: 6.2 MB (6229798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c881f3ed68b560c31b1e4c164f4674369a457f5047df27942be5ac42137a9965`  
		Last Modified: Fri, 28 Jul 2023 07:50:31 GMT  
		Size: 158.5 MB (158543797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f6df175cbbe57497a33c021ef1f2c48f6a35790f9ee0667beaa6d4af321950`  
		Last Modified: Fri, 28 Jul 2023 07:49:47 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
