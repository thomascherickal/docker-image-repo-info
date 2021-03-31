## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:8e0ad5c3f632cabcf2f95a046db51191d3ae5c1e49ca1351b4fff8e589d9480b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9f3ebc7a456e1c7306cbd5f264c011c3dbf677e0f429251000b32559db6d1da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61009073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec9dd671a8e96d6f1679110be7f7965944cf6d4295f95cf48622bbdfd1394fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:82eccd31b30d9f3b261efe9b759445da28a565a2d701d558a0c0f7688d4953bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58587438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444f4f9e9afd0ae14536d946ff9dddf5c8df4cfaa2da77b7dfe4e7eaf003f8fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:53:43 GMT
ADD file:471d7a5419df3b812f9a1b0b14c1bfbc2b8fc88652b66cca395a28af61a77f4d in / 
# Tue, 30 Mar 2021 21:53:46 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:55:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:55:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a6404a8305ff6dab0e0a06c0c4291401369422bb5ba3e2b49d5447049a0928d7`  
		Last Modified: Tue, 30 Mar 2021 22:01:23 GMT  
		Size: 44.1 MB (44091975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c93c80b72e9e001eb0738f044aaf49d57cdee5c4621e362ecc2ceebd6ae3`  
		Last Modified: Wed, 31 Mar 2021 00:04:47 GMT  
		Size: 10.3 MB (10333990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3d70057a6c48834905e9f7b2f91c1c66f824e2665b9704c701c726bdbf572e`  
		Last Modified: Wed, 31 Mar 2021 00:04:42 GMT  
		Size: 4.2 MB (4161473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:511734e3bab69bb7e44fec3aa03fd55047f50b9e059f9c788acdddb8114e2de7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55980857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba5e942b9802e4a72c86ca05992b3dcb78bfd42f346b23f6282deeac7c0804a`
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

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f5290693571bea7afdb93536746cb9b581504836842c7e234b614f71f0306dd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57475362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195d1609cc4314cb36bd320303dc1c35bc7b2d4068867725497bb789b811cd73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a5faea88d3a31bb9029e78d51932b4624ebdcebfe4fee38e92465de8ec17d03a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62000145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f0118e3706e26bcab4d4ebaeedf970657b5a5d251a0486e59e133c4e3eafa90`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:30 GMT
ADD file:1df7a35a36c49061902cf634a894b34a55a9c020976547cf6d2dda96879854bc in / 
# Tue, 30 Mar 2021 21:41:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:667bc6614d317ea77075a4e2f4ee7ef7d7b696f50d426cec38048d3ca20f1aa1`  
		Last Modified: Tue, 30 Mar 2021 21:49:28 GMT  
		Size: 46.1 MB (46098556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d5e0a8886ebed26c676639259bf05d50ff3b0285ea4b8afd1492ea424e7ff`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 11.3 MB (11336592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd0bba69d5c567fef7e770351f3ae71bdff83884b1d5af86d4dcd6ea6ff7a9`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 4.6 MB (4564997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
