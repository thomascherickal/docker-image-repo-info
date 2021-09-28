## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:d4c948e5878020fc64c13e27ea28cf8030b7338e21bf73be07c56bc16473407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e042672f1de31e5ecc5bbf7df2a9eac7d1cc012a5a620ec3b0b5aa0ccae9e610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110781699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49daeb05d0974f360f43581a6691f08a5b169f1813fcc867a41293f40e7e4b5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:04b27e881f1fd6778bbb2d8d0b731458d3000b2abe8f7e2259d97617f39b893c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f2d0d5fb01b8578c38085b55152fac616466476f7c3ccc7799c0082b32cdd4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:55:20 GMT
ADD file:838b3017c5e14c9c2cb8e2beed881284e402b04a3fa00d6660af0164a62e9aac in / 
# Fri, 03 Sep 2021 00:55:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:44:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:44:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:990f81d6b076b231549a6d1c9525983e601a394687d6f34de260e0319bf53ccd`  
		Last Modified: Fri, 03 Sep 2021 01:13:22 GMT  
		Size: 44.1 MB (44091687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddec37b68b0e6232e73d38bbe052e6804a945ec22ed1da8856b3a94ae6967d5d`  
		Last Modified: Fri, 03 Sep 2021 03:00:36 GMT  
		Size: 10.4 MB (10350740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad7b012ed89a45c8d41452eee67434c831c33349535d3edc940d38f72a814a6`  
		Last Modified: Fri, 03 Sep 2021 03:00:33 GMT  
		Size: 4.2 MB (4161371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523728c66871b711f3e47439ee3a65721b15132ee3a78cd31ba598a14ef8e4db`  
		Last Modified: Fri, 03 Sep 2021 03:01:25 GMT  
		Size: 48.0 MB (47984014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8d3af45e79c9dcf3bc112dec67ae54ba97b8f2ce73bd55ac2bc983d2c670f416
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6acf122dd31ab2017b039bb761829e1902857a5af092009272383beea24072`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:04:44 GMT
ADD file:f3526ca980237b2ca5289ca7a6c67760fc5726ce3c325de10f3f3111c1d4bdcd in / 
# Fri, 03 Sep 2021 01:04:45 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 03:03:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 03:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 03:04:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aba3565275cf0ab544dbd3d27fb468b4682c0273b64b5f3d8c8fe06ca3467237`  
		Last Modified: Fri, 03 Sep 2021 01:21:57 GMT  
		Size: 42.1 MB (42119584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d7b8704af020029979f5a4bfc12eaea904235f452d75b61476aa90807ec20b`  
		Last Modified: Fri, 03 Sep 2021 03:22:05 GMT  
		Size: 10.0 MB (9951651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef77f0ed56b31ff8d57db5fd7149505dac04ef41f4919d6a59ed5e3725a6f4e`  
		Last Modified: Fri, 03 Sep 2021 03:22:03 GMT  
		Size: 3.9 MB (3921218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612339c5de82d58230628e90ab66882406b5153ad5eecc07c42f9418c7404e11`  
		Last Modified: Fri, 03 Sep 2021 03:22:49 GMT  
		Size: 46.1 MB (46125736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9e7864c0aab885d9c738e47641a9312fabba6b395daca3b76306ba2a0fce0d8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105228812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f625f1b11b3ace5c716eb8b6715da356e83bbc04c61e0f84f0048c5f9360ff2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:34 GMT
ADD file:3a77488ae0a72e8fd504cb1354bd111f38a4fc9f3e541ee7ebce3ebc4eb9dc49 in / 
# Fri, 03 Sep 2021 00:42:34 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:36:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:36:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e98a9e31e599c3e38ecd12cf6b8493f4268c371026bae6d2280da418009b5bff`  
		Last Modified: Fri, 03 Sep 2021 00:52:57 GMT  
		Size: 43.2 MB (43177996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f698e334a0e8a436e04b2ef344b0ada5761244cf05829ece406e740b750b1bfa`  
		Last Modified: Fri, 03 Sep 2021 04:44:45 GMT  
		Size: 10.2 MB (10215862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eef9137c22a6fa0d9b497479b8c3ba0d211b5f01fafd237e4dc3419146e22a`  
		Last Modified: Fri, 03 Sep 2021 04:44:44 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2efbeafbf19f86b2e28e71c625638965320adacde43d09588d14e4f5cb2461`  
		Last Modified: Fri, 03 Sep 2021 04:45:05 GMT  
		Size: 47.7 MB (47738412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4b82ca05cfcc3d4db445a63e663876f11fadf48c6c04ff1efffa3cac11c5ebc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40551e8c31ce139ca23f251e1c53f664d21686d1c874cfc000837b7674b68dd2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:30 GMT
ADD file:46f32d47386428deefe487caf3a07dcbb3fe2f2e89abd3b63cbe7e9d31444ec6 in / 
# Fri, 03 Sep 2021 00:42:30 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:15:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dadb58ce47b39e4093a503cf3b5a3fdb91180e4b16e14c1146b7bb865336d6f5`  
		Last Modified: Fri, 03 Sep 2021 00:52:52 GMT  
		Size: 46.1 MB (46097308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd444f00c798bfd4f9e617154309c372e8d36842dd1b1941d71becd772ddfcc`  
		Last Modified: Fri, 03 Sep 2021 01:23:40 GMT  
		Size: 11.4 MB (11353014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0571d1af33e8ba8e01d8c5f2ff9b4e4a3bd4bd88c459d958bfaa57077a0a3f6a`  
		Last Modified: Fri, 03 Sep 2021 01:23:39 GMT  
		Size: 4.6 MB (4564992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dcaa4b267350835d07fbb9cd12470a43123a18957bf035ad503417f9fe38ef`  
		Last Modified: Fri, 03 Sep 2021 01:24:06 GMT  
		Size: 51.3 MB (51265099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
