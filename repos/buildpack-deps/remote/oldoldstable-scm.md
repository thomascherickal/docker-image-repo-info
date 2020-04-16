## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:ecc75214b3baa4e18366e65c96d0ca6b835fb52ff8b16003c0f22b51f28ecafb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fbaa44e608f5dbef36a24d195a2d13bb323f779208233e53314f97ee807d1119
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115275307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3af8166e22f48f4d29f353009366782907ee9d345ca813f4cee400eb749e38e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:07 GMT
ADD file:06c434cd627b8970a4f3d8d76b36955fbf53b74db3f0ce29f1fc3b269c81f2eb in / 
# Thu, 16 Apr 2020 03:23:08 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:04:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:06:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3707da5d661028328ae23959ded4ecbb1e5ddbe2a4e8551cd5b6f90e90e6cbd5`  
		Last Modified: Thu, 16 Apr 2020 03:32:06 GMT  
		Size: 54.4 MB (54390842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a013c08ba606e93a8e6efa446e68ae82873c251f8d211d99fb2c3896cd7df989`  
		Last Modified: Thu, 16 Apr 2020 04:17:25 GMT  
		Size: 17.5 MB (17545810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3dd2434033ea5efd099d5168eee7856f41fbd7d636fe85dfb2a6af4bef6e2a`  
		Last Modified: Thu, 16 Apr 2020 04:17:58 GMT  
		Size: 43.3 MB (43338655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d6dfe84ce97c5fbb3cd4fdcc76ccd6e2fb0e8bf8e03f9006dd727d15c525f280
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110777238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03754948cf4b797dfb930395bf563796c56b0d6bd7a5f8a6dce52a4cffcd2dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:25:13 GMT
ADD file:631f76030613657eb3d82228323e5a3860b5141b58858b628bee342bd47d427d in / 
# Tue, 31 Mar 2020 01:25:17 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:29:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:29:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:31:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ebddd0cca47bf5452de875b55a7b0a10e182a550196df63972f211a03e9f7cd`  
		Last Modified: Tue, 31 Mar 2020 01:33:28 GMT  
		Size: 52.6 MB (52580205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e80167505cea44898f4dce8e6007acae3e6ccf8b0b3b62d514cb4d769474d4`  
		Last Modified: Tue, 31 Mar 2020 03:48:54 GMT  
		Size: 17.0 MB (17037090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962f7d2575522a8a0df557e93a9845753c76833c794b332df26816e3213f676`  
		Last Modified: Tue, 31 Mar 2020 03:49:15 GMT  
		Size: 41.2 MB (41159943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:17718cb62a06b3a8f013c386540dea1a4d55e356ec4149367435890bba15476e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f62c28dae6bca9ce485c37d627d56ba163f19718af5d8cd9ef14fc3e9d7d375`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:00:13 GMT
ADD file:0b08b600835a16058b725946cb7ae338fea6a14cf6998584f9728d2c62324f1e in / 
# Thu, 16 Apr 2020 01:00:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:44:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc084eacfbe394e053f99559ca63f9d660d60dad0b70a31347e5088af534b2e9`  
		Last Modified: Thu, 16 Apr 2020 01:09:20 GMT  
		Size: 50.3 MB (50304312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2753eba5d276059ffd460d19c6e651040079c4a18c7d6a93682bef3e285c0b9`  
		Last Modified: Thu, 16 Apr 2020 01:58:21 GMT  
		Size: 16.7 MB (16723352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff41b20f0ffb69690b5b8efa517a6db82e30df6bbb8a1ba31dda7369f437c9a`  
		Last Modified: Thu, 16 Apr 2020 01:58:41 GMT  
		Size: 39.8 MB (39777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:870d895727f5175803af7bfe4bf76c278a76e7bf088c79c55d7bd4927b0ca9a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118443886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4736dd2b1f9e0bffdaaf52b6f62621dd7e188eae62256e735c1f2669ead15654`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:40:13 GMT
ADD file:fc5ade2a561dca01c2a4d4035601db636d098801b5655a1bf239e8b706395f87 in / 
# Thu, 16 Apr 2020 01:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:23:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:582c227f31bedb5a1092c02e624ef551c8659052150d9e9368da891fffd1528c`  
		Last Modified: Thu, 16 Apr 2020 01:46:40 GMT  
		Size: 54.6 MB (54607914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1866a4665d6ee342c90adf77b23d7002ec3ef1fc701d3c2df2ca95ab860994`  
		Last Modified: Thu, 16 Apr 2020 02:38:43 GMT  
		Size: 19.9 MB (19855771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e614c5ad0e7f598900eb10a2560d248d97421d118be8b34cc663827e5e9b0f2b`  
		Last Modified: Thu, 16 Apr 2020 02:39:00 GMT  
		Size: 44.0 MB (43980201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
