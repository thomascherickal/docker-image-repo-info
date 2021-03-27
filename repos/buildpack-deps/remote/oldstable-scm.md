## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:70afa7e8f0b3e25034c41032201aa2a67280203f245e42f520101540e86caf2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:acdd5f8284383bc7883cadcbeb9e1594712904a0967c8c14dc387992fe89d759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110780201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43c2a352515697921860dbcc2ae7903ca5dd83b4ea7f11f95b475df97be57dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:36 GMT
ADD file:5f8ab4280b54d91475c84e497163ec05aabb5a9f9b9de687d38fda535ddc29b2 in / 
# Fri, 12 Mar 2021 02:22:36 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:52:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:52:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:52:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16cf3fa6cb1190b4dfd82a5319faa13e2eb6e69b7b4828d4d98ba1c0b216e446`  
		Last Modified: Fri, 12 Mar 2021 02:29:57 GMT  
		Size: 45.4 MB (45380216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddd031622b35dad4be68eec6ac0787b0394f37b3dbb600a04e8b2363297b8d7`  
		Last Modified: Fri, 12 Mar 2021 03:22:18 GMT  
		Size: 11.3 MB (11270857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c3fcab77df556f3a56ec3d2a5b5cc304f4c4d4341b6f8423dd86ebe5ddaebb`  
		Last Modified: Fri, 12 Mar 2021 03:22:16 GMT  
		Size: 4.3 MB (4342349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a403cc031caeb1ddbae71b9f7e47d7854415c8aa6f0b84b8e7be4b3db513867e`  
		Last Modified: Fri, 12 Mar 2021 03:22:42 GMT  
		Size: 49.8 MB (49786779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:419a188579bf4ece850aba483bcddd499c0ed789f453c1442a1eaa94fcdcfa6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106573696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7849a0b78145a9ae50a0ac5139c0f9c78c4d1a13188c9dd05e240e7f246ce421`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:55:39 GMT
ADD file:ba0bcff641608b2668ebc0a0a795d8bd32a275ee0bfd9e161b43fafccfa96545 in / 
# Fri, 26 Mar 2021 07:55:44 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:20:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:20:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 09:22:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7298374463f66e0dde12fde13b833e7f90c3f9d526420eb8a6f05dbbe3600d69`  
		Last Modified: Fri, 26 Mar 2021 08:04:13 GMT  
		Size: 44.1 MB (44091954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf04a4a71171f6c8b01836696265196f508f5b8482f81375e241b3d7569347e`  
		Last Modified: Fri, 26 Mar 2021 09:31:01 GMT  
		Size: 10.3 MB (10334011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2230286c48428bae6a7e9521aec8b20a46b92ace1087dffdb7719a92645f77`  
		Last Modified: Fri, 26 Mar 2021 09:31:01 GMT  
		Size: 4.2 MB (4161500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2426b855cc43ca6d9f692c0e7cad6d3e9df5576652e299cc60d0a45125a96eb`  
		Last Modified: Fri, 26 Mar 2021 09:31:30 GMT  
		Size: 48.0 MB (47986231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5daafbc13f03b51fa118bc95a954da16ba4f44406907b2ee34e6b645e4152867
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102108480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54aee3c7f7d7c19537f6bab1322a32a4560c7c1cb908fdd463f3c533117a9baf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:32:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f4a3c6ff8566959485607b47c6d4748a4e04e25a1b7d98c2e289c887074c9`  
		Last Modified: Fri, 26 Mar 2021 13:55:55 GMT  
		Size: 46.1 MB (46127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d155ce6c3ca991df86837cb64ccc080b84bd3abc90e1d33e6ed6425b2a853e7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105193160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bb63ffc0c35f1a09b49bef859ade80b919b516b8705b09d74ae2b18d3a00b5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:56:48 GMT
ADD file:3d59786321ef76584460518105748706e36cd0b833f1d542702f9e238073f63b in / 
# Fri, 12 Mar 2021 01:56:54 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:36:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:36:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:690bb835f855da2bebb5afc2671951a9cafcaae8e3751eaa3ef8536058581b9d`  
		Last Modified: Fri, 12 Mar 2021 02:03:51 GMT  
		Size: 43.2 MB (43177463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900d8bfcdd8c3d3bf8eef705080ae89efe5d9b24294b7d39c1c0d44f93dd47f`  
		Last Modified: Fri, 12 Mar 2021 02:46:19 GMT  
		Size: 10.2 MB (10184079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f83540a087edd442573d6168d03eb7e83cef27a2e34ece682ea441233733ce`  
		Last Modified: Fri, 12 Mar 2021 02:46:17 GMT  
		Size: 4.1 MB (4096643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef9c13609053a0f18bfd7ec1ca3e02fd48ed839084b2d58f79a51c9082893d`  
		Last Modified: Fri, 12 Mar 2021 02:46:37 GMT  
		Size: 47.7 MB (47734975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ce0e6f2f3eb2e0e660918b0d3551e9cdb580344a7ca22c6ea698d33be4274fc9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113265074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1143ca8436c7a38aa23ef309a78ae71e81b44b6aa2cc26b869762b73e482e6dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 13:55:57 GMT
ADD file:0a48869723941cb015604aec94e5f955449b86eca7c73ec978c3d1dcaf3517ba in / 
# Fri, 26 Mar 2021 13:55:58 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 22:48:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:48:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 22:49:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01c2b0829d8abcf8cd9012766b99919fd21d4a2c1fae4d9312b5716bf40ba27e`  
		Last Modified: Fri, 26 Mar 2021 14:06:26 GMT  
		Size: 46.1 MB (46098430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd034d6463d3d9372f405b356a0e09c553416c4c875ff58bfc709940c165f19d`  
		Last Modified: Fri, 26 Mar 2021 23:00:01 GMT  
		Size: 11.3 MB (11336731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9889d71e348186e773160024e7d403e8a0ac99f4fd04c26eb0b04023c8eb7da`  
		Last Modified: Fri, 26 Mar 2021 23:00:00 GMT  
		Size: 4.6 MB (4565051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce5dd564d786a704453c35a01a5b0f08bf43708c6479077ea140e47ce9d1a3`  
		Last Modified: Fri, 26 Mar 2021 23:00:31 GMT  
		Size: 51.3 MB (51264862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
