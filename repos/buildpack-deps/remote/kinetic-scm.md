## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:4fdce5422784f7f392f88f4f20328475a4ef70c4ecbafabe78b378164011cb3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d04920e171fddca160ba2431b2421bf49b424767a2a15f5be91bb9d94f21bb2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77583500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ef1de29f63807a6093e6af698173335a81692ab641a3e02e63bc9df42ea5f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2965cc2f6b4e99430ed3e5dc6e19cff61861fd39ce9247198d0446c4ea18da12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78226975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf87da53eb6a1926ffac398aa2b41ffc1c7ba4e19fa01b0c1e132a9fcfa6d7ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6de355c79842fa3dc42395bb16ac892a9aea9172ae100e2b7177ee9045f7b023
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76182409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56880101245c2546da39fab260b70f57dede5f401bdef477f46562d77e99100d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:29 GMT
ADD file:2496d47197031551828443c95a5e1dc6bb6dc7855695a8470f3ec96e8441e76b in / 
# Wed, 05 Oct 2022 00:02:30 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:33:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a768b6c77af7a723d25d349fe4a633e82e8ad41fae270b2bbee8849bb840009`  
		Last Modified: Wed, 05 Oct 2022 00:04:31 GMT  
		Size: 26.7 MB (26690398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56476b006a508648b853d25af5afc829804e3d75931022c7583240f09d0c1b06`  
		Last Modified: Wed, 05 Oct 2022 00:43:58 GMT  
		Size: 6.6 MB (6608273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e10cd4bede843113d9336d39042872604d754220f3cebb42d6f4d05652dd7d`  
		Last Modified: Wed, 05 Oct 2022 00:43:58 GMT  
		Size: 3.4 MB (3389726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8841f74546971e6dc2a63f25ac58478259dab7f54f7f714c4d97bb22457ced0`  
		Last Modified: Wed, 05 Oct 2022 00:44:16 GMT  
		Size: 39.5 MB (39494012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:550c2c2854ecf1e4778c3db7e1e65d6a6823f3b9638ccf3f61c71c9f25f62883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88350466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dcb4471f6d56a4e60947ae0b49da48e269e4ed2b8979c7d0973d5bb744dda89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:41 GMT
ADD file:88a1f03ef21cfaa40a714986930314d37550633cb8512f4b6f8f181d8578923a in / 
# Wed, 05 Oct 2022 10:52:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 19:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:08:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 19:09:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21fc6649e0514e6dd480d6ec510ee3e255e841bc45eac6d3089ae5a1b109f126`  
		Last Modified: Wed, 05 Oct 2022 10:55:19 GMT  
		Size: 32.1 MB (32115528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a5df76953e60313a5de1b99d22c610ff4f6d792a2aa4df054a3d5e2e8068a`  
		Last Modified: Wed, 05 Oct 2022 19:21:11 GMT  
		Size: 7.8 MB (7752621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405ae789cd2ef2c1b80f14518be0bfae96a38c469b609ef2e8995182825097f8`  
		Last Modified: Wed, 05 Oct 2022 19:21:10 GMT  
		Size: 4.4 MB (4361276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e375c04bec6a143e973e0add25a0ba4b089c9d07ad7fafb9d34513f2d34e02d`  
		Last Modified: Wed, 05 Oct 2022 19:21:35 GMT  
		Size: 44.1 MB (44121041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ab238169f3b08dc7c08c8e3ed46e6ad74014ba89c7d7d398a9038687df3104a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78270889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bec2b637df9811eabf5c8c05afc79681031c55e2b577567a231be07852233f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e76025b8e1cd0c49120f5fef7b189ee72ef0293417db89af5ff36515226012b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dabceb577eaafe2baed96ae74298be8738aa7eb6def81236334da5ef7c4c6b76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:53:10 GMT
ADD file:4b04232627e4ab4441752376c6d51dbcdf07b65cadc7027da4c4cc79d37824cc in / 
# Tue, 04 Oct 2022 23:53:13 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:26:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:756b9b94f7ea9eda3168c766dd8c30136a2409b90d55b16cb335507dcc5e055f`  
		Last Modified: Tue, 04 Oct 2022 23:54:50 GMT  
		Size: 26.0 MB (26029724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777e01a92aac9f6f68b883738330b61f5dd370112f6443f44898ba567cbb938c`  
		Last Modified: Wed, 05 Oct 2022 00:36:17 GMT  
		Size: 6.5 MB (6475463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918aa0d020e12cbe864a35fb042a07a6069bd7e8dd270eed48961e8d5625b6ea`  
		Last Modified: Wed, 05 Oct 2022 00:36:16 GMT  
		Size: 3.6 MB (3625655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5628cde4bbda67e815888cf5a1d62f8a40e0b37be66e0725366f9129ad88da83`  
		Last Modified: Wed, 05 Oct 2022 00:36:29 GMT  
		Size: 39.5 MB (39548273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
