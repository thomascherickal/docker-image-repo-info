## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:d8e7741de8563afb6ee0265ef631ad670fc873bf0fea83f8e6458cfb540c4b4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:62c202ce5cf8cf05bcb2ba5a873e1590fb65fadeeb82a6c0909b7dc0585d74f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128720462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c577bace026f3ec0ecea3874f32bad4f5b02436f6da5fe8a140ca47b896691f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:50 GMT
ADD file:1f62518cec36eb3320e38344c0d36779557214cfce8bc32eda000183a34a0ffa in / 
# Wed, 17 Nov 2021 02:21:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:18:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fef5443775fe054990b02e8f72c4c5bc7792c6a5bf6ef8df110873a81676a87`  
		Last Modified: Wed, 17 Nov 2021 02:28:03 GMT  
		Size: 55.8 MB (55758091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63aa91be04004e56a4d31d70c789eadabfebe392e2f76a862eaa2fdd70dcfd`  
		Last Modified: Wed, 17 Nov 2021 03:25:48 GMT  
		Size: 5.3 MB (5269763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f625d605a0450d800b57ca6e2e0662fba5094348ccbf581c053a485802ebe1`  
		Last Modified: Wed, 17 Nov 2021 03:25:49 GMT  
		Size: 11.8 MB (11756478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0dd71d7f2f690f062de61d743dd487108ccd38089c95218a295206a6c68c3`  
		Last Modified: Wed, 17 Nov 2021 03:26:09 GMT  
		Size: 55.9 MB (55936130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a6fd6b6ff59a9e3a097d8125f6ca8b78882f804f0ca5bec557784676e4d379a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122358029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4f3e109e84ef325b2927539c9c569367e50198086ed8d72be40ef36742c34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e25517d9e4d5c71b0fd71f8672be17b1407629cf364b7b4c875a48dd1572d1d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118543731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22e7df05fd0bffeca4c0755b5570159b2a6f9ae77bca4317c40c4257b7e6e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:49:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9096006210de2acfc2854bd14870e0046c7c41610d75f402e14c7fa186a10`  
		Last Modified: Wed, 17 Nov 2021 03:10:01 GMT  
		Size: 5.0 MB (5029921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864516b2a87655fdd355f203892d84f29fb0f553f371f37e7027ceb5017ec34`  
		Last Modified: Wed, 17 Nov 2021 03:10:03 GMT  
		Size: 11.1 MB (11067071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e207fc56e058029a1aa1e0cae4ac127bfa621c4e822edde8fdad43037978ac`  
		Last Modified: Wed, 17 Nov 2021 03:10:51 GMT  
		Size: 51.6 MB (51586431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:53a7a85e1527f3f5ff060a2ff698f4e3a9caac5c37093687549c9e53d17b972b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126475529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df6c461ff7e30ec56e5d3be632b5e2a2cc49820f5613b9aefbc7cb7e356d7b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:36 GMT
ADD file:830671e1709a0164ca60ad1012d3d0202e7e63c74bdbec7df54f308a4d4c8b11 in / 
# Tue, 12 Oct 2021 01:42:37 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:01:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:01:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ed37bc205e0aad196bfd6ba235a1a5fba10e02175afd192c816df6457d06c75`  
		Last Modified: Tue, 12 Oct 2021 01:50:51 GMT  
		Size: 54.7 MB (54702895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b442bf08aba463a082cfb5ba913edb463c12ae6317b7e033c0267969b5e384cb`  
		Last Modified: Sat, 16 Oct 2021 03:16:42 GMT  
		Size: 5.2 MB (5204078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4710368d7f49ce5fcf204014ec59b6822a946d51959e5855d9678f1db1d652c0`  
		Last Modified: Sat, 16 Oct 2021 03:16:42 GMT  
		Size: 10.7 MB (10682376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee59fb18000efceec03c96ac160ae405c2816694cfa49f0ef85a63db84daaf`  
		Last Modified: Sat, 16 Oct 2021 03:17:01 GMT  
		Size: 55.9 MB (55886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:733772bac49de30e8a05b0ad0e7d0340e5b5089313a4dfdb7f57a6d60552b79c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130503569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41174274a4fa2d6806ed55fabbfd91e97b22e8a8178e2412b0e819bceda895d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89ffe14200fdc5ef8d32d228027ec8f1cb4f4e336dc2f12e03c9542883696b94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124925003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8df2d03f5cb58b6b7196f8d8fc1afcdfd3bb588a4c45471bcb87e4b697d146c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:13:27 GMT
ADD file:27e1d46380432bbd287bef3c049b6707a409fa2f49f07e76f4826c6ee57cfca9 in / 
# Tue, 12 Oct 2021 01:13:28 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:58:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 01:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7afe2e09744237d99a12c5f86f33ba55800e5acee482662abac2c64c64a7824`  
		Last Modified: Tue, 12 Oct 2021 01:23:41 GMT  
		Size: 54.3 MB (54313468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8be3dfdc1ee7ccf4465ff4d91c782f9ad2d795bd9ea4965953382190a5626`  
		Last Modified: Tue, 12 Oct 2021 02:11:44 GMT  
		Size: 5.2 MB (5177464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f028726b389731d6d9e30d4ef26719ac3a44889d1bd0681ebbf11f085178373`  
		Last Modified: Tue, 12 Oct 2021 02:11:46 GMT  
		Size: 10.9 MB (10904218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2076aaf953f38208fdacaa4098bb05224c1ede12a74b5ecee28db74cfd04ac8`  
		Last Modified: Tue, 12 Oct 2021 02:12:36 GMT  
		Size: 54.5 MB (54529853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9cb107173cfcf70286b43387a62f73d446f950ebf1d6ec736c213caee43c6b07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137168656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ed13442782d0723cce8315405a10fa6890398277e8cfcef4bfff32c2833bec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:27:58 GMT
ADD file:975422ef5390ff94fc050a84a9840e39188158f1c74f7b6dfde93829787b7c8d in / 
# Tue, 12 Oct 2021 01:28:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:23:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3794e49fdef56187e1a7ffe8a3c0d0dda8a5b5c159e370831000df5e5f638479`  
		Last Modified: Tue, 12 Oct 2021 01:41:02 GMT  
		Size: 59.9 MB (59889168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3a771c64c6b854d6abde14ad239e8808ef66674301b6a066df68b719b9ef04`  
		Last Modified: Tue, 12 Oct 2021 04:44:22 GMT  
		Size: 5.5 MB (5468996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a4272fe59063922ad53af8014c08c537807fbc8a6fe125f51be34de8ffc53`  
		Last Modified: Tue, 12 Oct 2021 04:44:23 GMT  
		Size: 11.7 MB (11654490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97493787213daeca4485b87abed722776481493a73f647e2d70fc24c1d0efd7`  
		Last Modified: Tue, 12 Oct 2021 04:44:45 GMT  
		Size: 60.2 MB (60156002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8486f624b42b956b1401a5bd240b03ad282ea1e54edb5242ea846893478a20ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119790274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b441fc86b4e2662aeadd8e308872b18de076f1c73c976e045a69988dcff041e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:14:24 GMT
ADD file:9ce8adafd95fc1e31db924edf473abf22a68101cad20cd078c35db5fa719b34b in / 
# Wed, 17 Nov 2021 02:14:27 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a35675c997377ee8bf94b0a94460a6d2fd72a26b5c7fc6194b13ae99da869125`  
		Last Modified: Wed, 17 Nov 2021 02:30:42 GMT  
		Size: 51.5 MB (51522304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6561ec3264f30875424c0937b41795ce70f58306ddfe766af2fcb7d266b6a6`  
		Last Modified: Wed, 17 Nov 2021 03:35:29 GMT  
		Size: 5.1 MB (5080232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f12be064689662dab642f65c8e821186c7247cf7ea84901a22b9e2584d51ee`  
		Last Modified: Wed, 17 Nov 2021 03:35:32 GMT  
		Size: 11.1 MB (11140508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077cd6f4305eeccad12d3a65baeff88b63dd35ab2735a8b6ca9d8f523e0b6a0a`  
		Last Modified: Wed, 17 Nov 2021 03:37:41 GMT  
		Size: 52.0 MB (52047230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8e5535d8b76c576ccc669d4f642fe2ed78be80df9778331222b1c87425845db7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126169798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6223c90d2c69ea15d0c2c6ca6033b860ee5f424c5d543919e86bc305d827047e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:11:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:12:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634664d8b893813a04761069646d85aea7164717481b8c7e3f500e4260fc39ee`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 5.2 MB (5248300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1780c6b7bcc6484f6ae6602c37ffd3bb2c9aad27b1b2587b796a5824e8b6575`  
		Last Modified: Wed, 17 Nov 2021 03:19:03 GMT  
		Size: 11.6 MB (11647079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bd04c7a7df4cb7de2e064bcfa156db3e89664ab5448cf33cf12043705f4f5`  
		Last Modified: Wed, 17 Nov 2021 03:19:17 GMT  
		Size: 55.3 MB (55308755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
