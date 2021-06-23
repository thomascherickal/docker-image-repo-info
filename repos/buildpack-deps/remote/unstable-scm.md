## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:f847fdb9f5954487e043d07eff6921ab59d5b651f96ced8acac13f343d377c79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:afb029322d4178a02dc3b018ea6be5b78ddc3a646d84f9afcd215ccc38516283
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126205019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4fac7dc096ecd81fb205f24a2fcd62f82f2c576603b605696122d3efd67b6fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:14 GMT
ADD file:5745436941906af011c9450820c7baff61a091235f04da258ba218ca450622a5 in / 
# Wed, 23 Jun 2021 00:21:15 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:54:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bbd4da8ff6e19a9b86585f9b55dede690ca6dca9f96d946fa1fb6456182931cd`  
		Last Modified: Wed, 23 Jun 2021 00:26:45 GMT  
		Size: 54.9 MB (54902493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0246214aa0ecb6ede7631e54d50bebe607ad610e577d4fbf6857d6b158e7dbf`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 5.2 MB (5170501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35d77eb31156f1996620962d6772ae81841ad63c839af8f4841118c8410fade`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 10.9 MB (10872573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c94a6468c400151537722b4a6b82a7e4fe16655ef49643f3ef4c591fa91fe`  
		Last Modified: Wed, 23 Jun 2021 01:03:34 GMT  
		Size: 55.3 MB (55259452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:50edcdfe6d77956d4011ded273d9ed94c236d0c28d770119512789ab9888b548
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120962130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99bb0ff7017a339a30103bae98a805c2909a15aa998c7b33825dd3864f489291`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:57:58 GMT
ADD file:74d49eb3680e0d1e7268c77ac09aadc6a9eaca2541a1941d02c05771fce80430 in / 
# Wed, 12 May 2021 00:58:17 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:55:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:55:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 19:56:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992a8499bbce77a1397237914a5f442e2a2d90912c4dcf8d75ced68fa669452a`  
		Last Modified: Wed, 12 May 2021 01:11:33 GMT  
		Size: 52.4 MB (52438763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c41d940ed14742ec6f26b83d52bccd7dc9e430c1dda8f4e8acdebb898ff0f`  
		Last Modified: Thu, 27 May 2021 20:06:51 GMT  
		Size: 5.1 MB (5074040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37054668f2f5a38fbe90534d3d0080b9438fb37e6c74493f206211677ac7fe91`  
		Last Modified: Thu, 27 May 2021 20:06:51 GMT  
		Size: 10.6 MB (10571286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443380432daf1d44bb7dda7f7ef3ede16dedb3892444726dc30dbc068156e47`  
		Last Modified: Thu, 27 May 2021 20:07:20 GMT  
		Size: 52.9 MB (52878041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:99c88c37d62ea8e86a81856a4e33ec7aff19eee3757fcb4961556a2287b62700
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116084478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f527362fb7e4714c51659693b1558fc09c61e3152d543167a7538eae1367d2f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:08:03 GMT
ADD file:45a139d5ba2871d3a6f990263a8fdb68998d0e072f5c70f796581383ed107962 in / 
# Wed, 12 May 2021 01:08:13 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:42:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:42:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:43:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:187ecf03b42c9078bbaf7c041564e40178e23f795d23634e11536955cfc64143`  
		Last Modified: Wed, 12 May 2021 01:20:07 GMT  
		Size: 50.1 MB (50098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4246453820c5b02c5c8b00dc0dde6bfb94015029c6b8005d49ade59af59c0f9f`  
		Last Modified: Thu, 27 May 2021 01:04:58 GMT  
		Size: 4.9 MB (4935074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9c0bc52453d252747af83975a8f1a58fe5bf2a18c4d879befd805239279f6`  
		Last Modified: Thu, 27 May 2021 01:04:58 GMT  
		Size: 10.2 MB (10216618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b443e7da95eaa262c0259ec871bcc330143ddd0e04dd971d0f5b7f936a1ba7`  
		Last Modified: Thu, 27 May 2021 01:05:27 GMT  
		Size: 50.8 MB (50834521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f1acc49c42f6372c4266b5486c5aaaab1a043f193c5cbff5455ecbe0709bb68f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125024342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308e7757bedbe74ba23302ac1ed059d5c862cf8c8bd25f632fc9a920885adf62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:14 GMT
ADD file:339319b02d36af7daf322a0b1295cc9416a58c021a5f5ba7a504f28717588cea in / 
# Tue, 22 Jun 2021 23:50:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:26:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:26:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:26:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e1aa4e0221ceafc83fb2f0929a4a51d5784e6bd00ecdfc3672853b28868fdf17`  
		Last Modified: Tue, 22 Jun 2021 23:56:31 GMT  
		Size: 53.6 MB (53586541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7626ab4adf6f17b187ebd4dddff8961986d7954ecf61d62b69eaa7ced1a128a9`  
		Last Modified: Wed, 23 Jun 2021 00:34:41 GMT  
		Size: 5.2 MB (5158799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f68a62ea25befd0307cf6cab1bf22ed625727daa8fcc5c452219a0bea940c1`  
		Last Modified: Wed, 23 Jun 2021 00:34:42 GMT  
		Size: 10.9 MB (10873185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6612ca213cc17f4e7c8e850bbd08e3342a7fb58ff637b59bc667f3bfb4792eb2`  
		Last Modified: Wed, 23 Jun 2021 00:35:03 GMT  
		Size: 55.4 MB (55405817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6659db0ec76e1ce8c3435017e4d243fd35cd99bb22d5bbf6e4d7e37c199ad13c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129131440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab03a0a89a12e2955c80614f29f214b564bb762e4c6374843bf1290af24ee3d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:40:18 GMT
ADD file:20378fd7bc859874d8620bd807402968cbe571a1ca281d0f344392ed5d8af55b in / 
# Tue, 22 Jun 2021 23:40:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff9feaae647f307940e0b5cfdb30f3d3a877220cd3394859c1af4b3d653b2e97`  
		Last Modified: Tue, 22 Jun 2021 23:47:46 GMT  
		Size: 55.9 MB (55914853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5310b9c9dfb8fd34f5ff4cccb1d7af5e1baf20620d64357dc51a0e69717717e`  
		Last Modified: Wed, 23 Jun 2021 00:19:34 GMT  
		Size: 5.3 MB (5299879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab8c3b07912881a8d38f2ca51a04fef6fa1d22c0163da069cd226eec7362a07`  
		Last Modified: Wed, 23 Jun 2021 00:19:35 GMT  
		Size: 11.3 MB (11250598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66c7b3456d19d1557f96e2c7bf74716f3187c850af8e39dbbccf8890f4c354e`  
		Last Modified: Wed, 23 Jun 2021 00:20:00 GMT  
		Size: 56.7 MB (56666110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:96773b4f02300d6e483feafe2afa795ee4bb758038c1dc708a651bd41841cf3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123221813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d20a999706ac9c6584d98907547ac8b0c92a5a65e4fc7c59c630a0aa5199437`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:56 GMT
ADD file:723b0881c85ba05a782aae0c0dfbbca4283e1a595a167af6a9a9b23b34916226 in / 
# Wed, 23 Jun 2021 00:09:57 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:46:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f938924a38054ec92bd31be4d18e4f654308796e5e915428065faea9385c73d`  
		Last Modified: Wed, 23 Jun 2021 00:16:36 GMT  
		Size: 53.2 MB (53157176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df9715e9403d707b9879b1f23718b1730cb5cf3feb4f483c137a321c7a2dbab`  
		Last Modified: Wed, 23 Jun 2021 00:57:10 GMT  
		Size: 5.1 MB (5129996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6704ed06dc069325a9235d3c57db6d14a34623f005bd10aaacc4acb2b42585`  
		Last Modified: Wed, 23 Jun 2021 00:57:12 GMT  
		Size: 10.9 MB (10873312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdace0ce09b260021353f35b35cc0d8e2dc930fe2d1cfb3cbf0cdc51c6f5c681`  
		Last Modified: Wed, 23 Jun 2021 00:58:02 GMT  
		Size: 54.1 MB (54061329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b9945745804ad20563bbaa726f0e091eda2b480a05edf8b915a39da8c58ca558
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (134976459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2de03d4df2c5fc49731dd20433b2632693e12e425d624561b089197958fc0bc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:35:19 GMT
ADD file:7d2dad47f7990dd0f8ed0b034505aa9c7d8afbd94956f80bb57feccf6f7e15fc in / 
# Wed, 12 May 2021 01:35:33 GMT
CMD ["bash"]
# Wed, 12 May 2021 04:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 04:02:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 04:04:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec00b4432728c9f962251efa3d91b6e0339e74ff656fbaad7adad52ce998ea8c`  
		Last Modified: Wed, 12 May 2021 01:45:35 GMT  
		Size: 58.8 MB (58798847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbf7f2f224053db3ca18ebfb195a650ed240333b2b7bc423c9a3190693e63`  
		Last Modified: Wed, 12 May 2021 04:22:23 GMT  
		Size: 5.4 MB (5419993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbba1e29d2e9ae70bab4c22a5dd913b1657725f350d6f9c4130d0f30ddc06ba`  
		Last Modified: Wed, 12 May 2021 04:22:26 GMT  
		Size: 11.6 MB (11625707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cc000b70a733d57e8882fa72e96ba17fb8f09e9b18b39bc5dfb02aa1d8b7c`  
		Last Modified: Wed, 12 May 2021 04:23:34 GMT  
		Size: 59.1 MB (59131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b4914d3348b22608dbb7f53c0175f4097a519d722190219d289af0f5a9038bfb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123813015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce522119f0b4800d09bc6c682f013701346863b93f24461efa623285db348cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:38 GMT
ADD file:b2361f35b2807ada58f66b4f4f160b2133140a85db4ecd56889a15f080793790 in / 
# Tue, 22 Jun 2021 23:42:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:07:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:08:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:247ed76d4285ef2f620cc0d1ec3492f8a6d1b0cc613aadf4e236db73dc508cca`  
		Last Modified: Tue, 22 Jun 2021 23:45:59 GMT  
		Size: 53.2 MB (53184006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9061f67eb9da8a0f6f7f323fc5113c55d3782998f1d177170951d684d367502f`  
		Last Modified: Wed, 23 Jun 2021 00:13:01 GMT  
		Size: 5.2 MB (5152169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2261334caf31e69fc462c4f94347962e98bb4b7a074c0fedc944f1458fbd106`  
		Last Modified: Wed, 23 Jun 2021 00:13:01 GMT  
		Size: 10.8 MB (10763416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320655ef4ccf1f9b477d71c135860e6ad84c4248ddfdcebfca06d0fe6f6d1a5a`  
		Last Modified: Wed, 23 Jun 2021 00:13:16 GMT  
		Size: 54.7 MB (54713424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
