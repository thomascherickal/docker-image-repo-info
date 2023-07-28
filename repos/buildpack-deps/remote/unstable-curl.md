## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:62ce2147deceb641176e699ef9cfcb4cf84404fc6948310530f61e0397233823
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1444ecae199d3a84f514fffd3e96a07d956d068d696e22a6668f3a8b7b69bea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73558597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b07e6edfec497631a8a3716b0e973fce8f54eb68ded798958b4befa07050d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d1a9056c98835bada87f4138da4b902136cb795eca133e00ff0b1c407fb52bc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70080759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9b5fce7ee5621e0e2234d3e15d91216d47839ce7270d9e7ac54cf651eecc62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b786440d5fa9313cfe4c6e947e1e06bff0b361070ae00db02f93c8a902770278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67108518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f38aa572847a45b4cc64179b342a4010030a0cfacec4a3e125ba276bc94ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:168cc096593e0cdf7b4e13f9739eb5733adc9069d240de7ed0fe35aeb2a2d2cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73103142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344af7b87e9677178d16f959dfdde57f165ec1af4db8ab0e3a034476ef16a070`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:555e0c926152f63f4be81642923a7d416a6db8de6cdeffaf232ce9a51950f704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75427637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43878012a9d69af31988db85d06eed454cfed8f9f71f7baeaf892725ce675e3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9c445cebfd89383262612bba3ffcd90741aead0f8078a8c553fa99aa51180e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73116035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563c80671a9f694e8c110c810f67d406dc3c68ae2109676af03b778087a4bdc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5807b1f6748c228dc4b2b9be5b8dd6d43925344484a7ac9794dd5a809331ce1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79206895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985fda4e25a501fb5c76ae42a7c2ebc1fccc03a9dad9be7395da923cac261da5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1ec0279f9d18d011062cad1be25abd66e64da40536c135db02b31f9b273289a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73060723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af73a45fd027437fc482806008569b16e9a19209902b6ef1ead753d323426a3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
