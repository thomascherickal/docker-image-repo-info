## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:c56b97d1d5a13a0deccc3f06ce84cc25d289000f58c033e39da33663eb5a6d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1897d92f0c0450dea079a00f090ac723ba0393c31d8495f63fb3324d4c071179
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69541632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a7789e59b7819ec8fc1a3212b107cccf937b88e1b382a152a4b67cb4ce1110`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd0eff3468a08b4cdf12f032ff78080b7173e0fe025644e187e4ce067d8cec4`  
		Last Modified: Wed, 03 May 2023 20:12:04 GMT  
		Size: 20.2 MB (20242385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4aaa30c5bbd7b0b73dc13c4349503da85e18417dda9ec35c3902c457c2b090eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66501070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b591302fb76d72e49beb255e57ed17302a80aef37161e6292ff3fb42436ae7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:48:29 GMT
ADD file:1ecd266ebf23430d2ea2417b92ebee6029d940fbe99297183c4f811e24fdffb7 in / 
# Tue, 02 May 2023 22:48:32 GMT
CMD ["bash"]
# Tue, 02 May 2023 22:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbca433c216350213a8b219e118cb55f422acfc53f49c76c44e044b42a5c0aa6`  
		Last Modified: Tue, 02 May 2023 22:50:27 GMT  
		Size: 47.2 MB (47167199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66d6e362e78baa664a585ad9ce74e92a9cd5b5324a686fbee141b57914ff008`  
		Last Modified: Tue, 02 May 2023 23:02:51 GMT  
		Size: 19.3 MB (19333871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44704336c87e91e613b580441c6a06a0736fea01732edcd0cbedc566efabcba8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63595097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1698fb29d2d87b815d67f9f91c763c7cb83a3a0c4b2e9d00757574c67a6c79b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:28 GMT
ADD file:222aad59c348a6e07dd607ba4626497e12e5054fb651c9c30d5a4c5a8b3e4c82 in / 
# Tue, 02 May 2023 23:47:28 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:51:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:326cff266909348fa4e168fc7e76fbd52cc4855403565526a5ecd2e6bdb9d26c`  
		Last Modified: Tue, 02 May 2023 23:50:34 GMT  
		Size: 45.0 MB (44988072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece266fe96bddd48a6f52c611c3c18dd73bd76ad395d47a7b4780d7d1a3db628`  
		Last Modified: Wed, 03 May 2023 22:08:03 GMT  
		Size: 18.6 MB (18607025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9796111463b4c79b14f3f084bba23b7776022ba6ed5e038cc9eebfd9c5a3c8d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69384780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be416f518c531f887e5b6870a1f258b9576c16ef598623a8383d92ee0c57d51`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:25 GMT
ADD file:1af23b8894efa507a47bf873cf69ecaa5ea13b618cae85b8c46125af6399b4fb in / 
# Wed, 03 May 2023 00:22:26 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:19:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15c964cdaf05fdeddcf9bddd79eba05f71f2859fee9c193ba5d19a237f7fb92e`  
		Last Modified: Wed, 03 May 2023 00:25:01 GMT  
		Size: 49.3 MB (49345335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd2bfca96f059705a95bd29801b5c141a373826be0a739310df1a330c3a4134`  
		Last Modified: Wed, 03 May 2023 17:36:08 GMT  
		Size: 20.0 MB (20039445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f083a48376b420bc0959fe21d6155b36f928d9a4768a03b4a78a8ef56ae17810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71147432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3330b81570cd20628fea3356a707d1360ab4f330c620ecdefc2826b051f47da4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:26:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8545b061925b7947aa3804b00e02ce1598211815db9012baa3de88b1f22d2883`  
		Last Modified: Wed, 03 May 2023 22:34:45 GMT  
		Size: 20.8 MB (20825605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:99f1e29495aa5ab7875b294f1ebe79d29e32433b2a0a7e722ab8beef56abdffe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68862308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec294ef2a18e0f9eadd67ccbbdb0c8dd906122e18981398fd1af1fabe2f5eea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:29 GMT
ADD file:ff6384c951ff8b6254c1c1f02c689314e2f30a43e4b60dcbf54c82df826f734d in / 
# Tue, 02 May 2023 23:47:33 GMT
CMD ["bash"]
# Thu, 04 May 2023 00:57:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc6b7fd1001cc2b329d98b8ea6ca86f4be0bff6654b36678fc5fa01f2f599145`  
		Last Modified: Tue, 02 May 2023 23:56:18 GMT  
		Size: 49.3 MB (49301357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca8caea3847f25ff54de7cd1198b575da538ccd5f7daefe1af6e83c69a1a4c`  
		Last Modified: Thu, 04 May 2023 01:22:57 GMT  
		Size: 19.6 MB (19560951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:58f1263c1585fa9466471d324244587357cdfd375ab7b80afa1da080cbbf7f22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74893152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6be993ff92c59ff217efd0ece8fb26fa183b83e62c4567ef0e8a24179e3901b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:30:45 GMT
ADD file:25d67bdf8a8d7f1826107ec67b95338418561c0fd3833ca3065cf965e82b87f7 in / 
# Wed, 03 May 2023 00:30:47 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:09:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e614e0d26e774be63c67b7f9f168ad3982d113da743f11dd74fec77e268d7e0`  
		Last Modified: Wed, 03 May 2023 00:35:40 GMT  
		Size: 53.3 MB (53307301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2b7373c4795c4edf6191c6e8844069ddb2239c4fc2e171691720178d865cbf`  
		Last Modified: Wed, 03 May 2023 23:35:19 GMT  
		Size: 21.6 MB (21585851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69bed414ff2a8e7351d3026cc4dd72e1786e124f2c77cd0383bfc7cf2f00533f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67414990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9d99d3f0d47b58057494325507b6e4cac61f6bcb3d8a04f94337dc155fc5ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 03:41:05 GMT
ADD file:2b13279140b98de657b363865f9ee14f0c5c26df191533d1c5438dd1df5948ca in / 
# Wed, 03 May 2023 03:41:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:18:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f966d911ea531e8d55499ff0d85338412ff6e8012a1639d691e4bc5ecf08d42`  
		Last Modified: Wed, 03 May 2023 03:44:23 GMT  
		Size: 47.7 MB (47675931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b703e1290372b8e634edb4c545eb551bb21b99dec3a903d38695f60715cfd3`  
		Last Modified: Wed, 03 May 2023 22:31:03 GMT  
		Size: 19.7 MB (19739059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
