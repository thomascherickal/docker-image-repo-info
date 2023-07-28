## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:25608dbaf958268ace7d1fa7ae5f9b9ee3f9ddf3545bd6b2cfb9f604fb0cfe25
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db8046e6728be4a319bf8c9c7fc53191969676c1aff3dc192ecb5e1acfc6dd44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138245050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c9f688e3f355ba0028691806d887b635ae646386d3bf3d5b1b6cda070e4e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6efa412d16b908043ec01c4ac9ff7323c0f488dd5d7ea4b9b086f1e80350b9b3`  
		Last Modified: Tue, 04 Jul 2023 01:27:46 GMT  
		Size: 49.5 MB (49475944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad8fa89586d6eb7c1bf3add3cde8c80b2da78794ef30be11a97f2dad784809a`  
		Last Modified: Tue, 04 Jul 2023 03:54:24 GMT  
		Size: 24.1 MB (24082653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80dbf573225a65ee45360f0a43a08f5e1809ec65e4c5fd3634aa3c651ce0aa3`  
		Last Modified: Tue, 04 Jul 2023 03:54:42 GMT  
		Size: 64.7 MB (64686453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0841006a6e7ae7124fb49383c6e729393fe97fdd7d5a764ba2cf3524717ac5d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132387410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a1dbd93f213db0dc50fa2e522af5b935f1ec468cdef913e9ba7a9874021b31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b5934a15453e5e63936a0201a34b820f06d7c27f091dc017bac7d92e1e58d7`  
		Last Modified: Tue, 04 Jul 2023 04:30:42 GMT  
		Size: 22.8 MB (22758286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4231c799b91b6f2c6d3090483baafb52160bc63bb7459deb8ea264e4018f2d3b`  
		Last Modified: Tue, 04 Jul 2023 04:31:01 GMT  
		Size: 62.3 MB (62306651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ef3af5ff6fe6345574d568b9ba626175b69ded771ab30deacab706cc412c49b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127062025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c39f924f6ca9f00579aa7a0e37403b02cd47ce2ba59130218cfd6f5fd31a0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb3f60ee8390c8cae75e83a5b95ebc4f3589ca1af647965d02fe99b974827b`  
		Last Modified: Tue, 04 Jul 2023 06:21:50 GMT  
		Size: 22.0 MB (21984543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1e5d5a935736b670eec63e61b0bdcc50ea4bc384b4ef00a257b7d98cbe0f6`  
		Last Modified: Tue, 04 Jul 2023 06:22:08 GMT  
		Size: 60.0 MB (59953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6547b0fb05aa47c02279476c9c339b27a73ba686a8d964767bf51542e495f10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137764860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b44f02907bd19b65d492b7fc136b89c412638c71ddb02410f4c3172aa8847bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:01:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b52151d5bb774f3680f8697c343bae1b64b7308354db57dc6bbeb7d65d0964`  
		Last Modified: Tue, 04 Jul 2023 02:03:59 GMT  
		Size: 49.5 MB (49482570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e94cfcd9a2ac0ccda7b085606ef5174003eb543c68b5bf077a91230b8a7f7`  
		Last Modified: Tue, 04 Jul 2023 06:23:39 GMT  
		Size: 23.6 MB (23620572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12422f578439e0f8042c87a47638ea9651cb9d674e8c89b05c5e4d333833ca02`  
		Last Modified: Tue, 04 Jul 2023 06:23:55 GMT  
		Size: 64.7 MB (64661718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:08ac98188b4d99022ddf9f16dc0a488ec35f19e9d09d3930aef1e2f733ae81d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141945829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989e556ea04ee7a099cc0e1e2fa0719d9fbf6a8ce54cc152f9844ccdc9f46e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6611c0dbf9970353c5c08585b89e28e50531495ee733b7f098fa9c3501067d`  
		Last Modified: Tue, 04 Jul 2023 05:42:24 GMT  
		Size: 66.5 MB (66518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:776e2afd9426f5f202780c44cb0d6c0ed2e77466bbee1fe230f4f8b68bb0bbe3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136723315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57625595c83aae207b1a1028993f73dcc398eeefcdafe5589ab032b376a5fd51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:54:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44357c89fac3bdc147daa7fe48fcf65b83dae0a924631c0b3e9ddb3f7ad71da2`  
		Last Modified: Tue, 04 Jul 2023 15:02:20 GMT  
		Size: 23.7 MB (23660637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360a64085c52bd3ade25ff3dffcad4ccd2db7944aad983d6da8f5a3e148e1a44`  
		Last Modified: Tue, 04 Jul 2023 15:03:11 GMT  
		Size: 63.6 MB (63607280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c6db7b3d9b8b7b9461c958da7d9061423f995b3e3d3d4d9e2dfd8ab01cefab08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149354347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1705ece1fdfc0d296b55a24fb47d71cd633a54e73ff649b62e797ad1429ca2c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:38:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e4e6efa69b637e0e8ca00ddcae1aed23aef874a92a2904bdc6c9fa5b3212b8a`  
		Last Modified: Tue, 04 Jul 2023 01:27:02 GMT  
		Size: 53.5 MB (53474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b5bee4b9196ae6959902bca430113379429a2f075e1553977c6d0442f46233`  
		Last Modified: Tue, 04 Jul 2023 04:39:59 GMT  
		Size: 25.7 MB (25732481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347de1638edf48069dc551f9b7887a170d69f36e44b3d711a5f35da08e29100`  
		Last Modified: Tue, 04 Jul 2023 04:40:30 GMT  
		Size: 70.1 MB (70147452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:96941110e49ead9aca1f19c783cee74c1ba60437aa646cb579afcefb7ad4b433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136838024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21031b741572c9c946128adaf02584158a5ab375ff2bcf317eb2d6bf3597828`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:50:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dcb3b9eb8abea3e1994db2e9f2073832965384334d3e204d1df1e3dcd09cffa`  
		Last Modified: Tue, 04 Jul 2023 01:38:16 GMT  
		Size: 47.9 MB (47890767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d5c8c8644c840146ba18a3d20250a3f49997785afe106720a31e6e3bc0bdcf`  
		Last Modified: Tue, 04 Jul 2023 13:07:16 GMT  
		Size: 25.2 MB (25169956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac95edda4f2261a710fe6cece76ae1adadaa655ad92be633a48ffbfffceaba9`  
		Last Modified: Tue, 04 Jul 2023 13:07:30 GMT  
		Size: 63.8 MB (63777301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
