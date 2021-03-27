## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:e00aa273bc961e55692a3b511d731c9770ba73f518fbaa89ac8ac38ac4fe39fa
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:352c44ab804db39c460a0233e5f5077651777045f2e4e99c1ffaf0ef96f85f0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70839292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8fffc62f77957bcc9d59dc182f1db8e392f65f8e28bb44f33fa7c89dd86f41`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:21:52 GMT
ADD file:719f8702f6aa56e8ad69f574e924fdf062e8fdc72584f70aaac387be5e1d4a51 in / 
# Fri, 12 Mar 2021 02:21:53 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:51:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:78c7a03f25ec710f7b6b9ccc0ee40eb1871016252eea6df272c68389f18d30a5`  
		Last Modified: Fri, 12 Mar 2021 02:28:37 GMT  
		Size: 54.8 MB (54840531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b278fd0013a1b4473879cb9b2035cb02c05fa6d0900c208a8ef34a515c8b3aa`  
		Last Modified: Fri, 12 Mar 2021 03:20:36 GMT  
		Size: 5.1 MB (5136354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30451e23b656b5f6aacafba452dc7ed84b576095192b81dad42df280fb244c5`  
		Last Modified: Fri, 12 Mar 2021 03:20:38 GMT  
		Size: 10.9 MB (10862407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6e18a8a651c2267bac19d4c6576060816fa4d1c0c6d76e3e118554484c9b011b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68033745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fa84b6bd46bbe5d90833e25348d6cae3b6bec52152405dc10c5a0569eb2bf7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:54:14 GMT
ADD file:ac1ac9f39520995697d7545a4221ddb94e841eedef2eaa8bfc265b3840c9d873 in / 
# Fri, 26 Mar 2021 07:54:16 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:15:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:15:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6ade6f33ef6b8c4fc72e7adf3004838c72714ea31573c675126f6144bbc650e`  
		Last Modified: Fri, 26 Mar 2021 08:02:48 GMT  
		Size: 52.4 MB (52402425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59c5c8b0fd74f36c82afb1a6f410dc3d75f681362b9f141a9904658804af12c`  
		Last Modified: Fri, 26 Mar 2021 09:29:14 GMT  
		Size: 5.1 MB (5060923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f841801148a4983446f3f0e72c194c22a654c192eac11f102bc7f05a2e5f6c7`  
		Last Modified: Fri, 26 Mar 2021 09:29:15 GMT  
		Size: 10.6 MB (10570397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:60f29a333364b10385602348bffaff3e46d640c57f5fe52d7140da5951cab9e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65210037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcc3601f76a9fa9ebe4cd36e26b3616d499c0e12b3c7571f1a2e7ffdfae425f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:20:34 GMT
ADD file:f0720ec9bf7f39f48d23428e3a1efab23881784e0db60db3031465e45c1d4893 in / 
# Fri, 26 Mar 2021 11:20:38 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:26:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9215022a83fc46d1d35467f5bc69faee0fabb5fa515b7fe907a7f483cf1e6223`  
		Last Modified: Fri, 26 Mar 2021 11:29:54 GMT  
		Size: 50.1 MB (50071169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c633ce4b5971f906b64dbb1f40d78e435bd4f582179e60994bc399bf45ffe158`  
		Last Modified: Fri, 26 Mar 2021 13:53:35 GMT  
		Size: 4.9 MB (4920691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbcabf672b68dab52cce7bb41819db259dd2a29a05c53c36a0e536ac293ad49`  
		Last Modified: Fri, 26 Mar 2021 13:53:37 GMT  
		Size: 10.2 MB (10218177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e6dc22ae4dbcd6da98dc98203beabc9abe30a87652415629a6fa0f8c62772e7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69515550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f2c8271961e2ec1a219f33612548de734e46fd52c6041e115a1937542eab1f1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:55:07 GMT
ADD file:e98b46fa08e28b488d04d4429e536292413d7b6dfbd8a34310c44a6b65b421e7 in / 
# Fri, 12 Mar 2021 01:55:15 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:443483bbe5c8ae014cc3cb8df57a0b708d2b55560844a100ea84ee50c9b1736d`  
		Last Modified: Fri, 12 Mar 2021 02:02:40 GMT  
		Size: 53.5 MB (53528745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595d36f863c2eedb478cac05b443a7facc8fbe6215c6ea34f6e78566d92db8d`  
		Last Modified: Fri, 12 Mar 2021 02:44:57 GMT  
		Size: 5.1 MB (5125646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162a05b96d3ad03a4a6a47488547154bb54acaebbb89c3308feb6fcb9e7182cc`  
		Last Modified: Fri, 12 Mar 2021 02:44:58 GMT  
		Size: 10.9 MB (10861159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8bf64fd9d9962d0c8d8c73e0a7ba502954cfb553b5598fc52b34ddf2eb5630f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72411010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b2862086d7b6e68f3a1b680beba33b6da16ede0960dc26d5a2f382b57b559b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 13:55:01 GMT
ADD file:325ae30975853b6389efde932aad38dd1eff2d79da625d4986da0e4690222e98 in / 
# Fri, 26 Mar 2021 13:55:02 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 22:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:45:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0f257c933d0ea6db1761240613e31039e161f54a3dbb897ce7f0da89b673a0e1`  
		Last Modified: Fri, 26 Mar 2021 14:04:49 GMT  
		Size: 55.9 MB (55881747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f0b66f608bc78a5f86e42e06190e29ff50df3d9076b8641d56d498c69946`  
		Last Modified: Fri, 26 Mar 2021 22:58:21 GMT  
		Size: 5.3 MB (5280228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949c2a8ae70678580d6ab562e1cc96e6698fa81a6e115fc69251ddf840983125`  
		Last Modified: Fri, 26 Mar 2021 22:58:22 GMT  
		Size: 11.2 MB (11249035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dcae6f81efc18d2770aea0370112f038f75c07d4a7abd5aa00b0d2ce9ddada9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69110727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a30bc22ba8f06ddc7b59de03281d6e821e34e25e650d21e6d423ba649803aa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:10:22 GMT
ADD file:45a8dd112a282d4aa23c7808fe9a53a90aed8669a8c0886cbd1b014e6f666e5c in / 
# Fri, 26 Mar 2021 08:10:23 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc0d626a86c29f3dd61b7699812357277c6ad4db66ed29b70e541593f9a413f7`  
		Last Modified: Fri, 26 Mar 2021 08:17:18 GMT  
		Size: 53.1 MB (53126824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dbc70ea4ba58905300e32d855fc4d13e3e008870c30e837cc6f6dfcdcab138`  
		Last Modified: Fri, 26 Mar 2021 18:34:02 GMT  
		Size: 5.1 MB (5112937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41493924139fb5a5080623341557e04fd10346da8a0160b092abe10a70a9bd68`  
		Last Modified: Fri, 26 Mar 2021 18:34:05 GMT  
		Size: 10.9 MB (10870966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8894049f8ed64a860940038abc63a43b95d3fa093b76f77952b16ace4465aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75802995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c30f249f18192d3d96b12bb66ee72e2898db21200184dc61254975412e8dab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:45 GMT
ADD file:7106c38838d3049ea5f78c190ea790f58ea352546fd1b55d2b07a152c34377c3 in / 
# Fri, 26 Mar 2021 15:14:59 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9927b5cbb0465e067777696ede5217a35993b727460cf5c92037d8823b48a09d`  
		Last Modified: Fri, 26 Mar 2021 15:22:31 GMT  
		Size: 58.8 MB (58782693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58a377d45252b512386356a873c76bee0b1dfb06189ebc9b0b723496f735b20`  
		Last Modified: Fri, 26 Mar 2021 19:47:59 GMT  
		Size: 5.4 MB (5399498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6380788cb9eda4a73e189b4139db3eda3a7b9f06d4e61e07160541bdec59499c`  
		Last Modified: Fri, 26 Mar 2021 19:48:02 GMT  
		Size: 11.6 MB (11620804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:693f4d2124b327f9987ce00fbbff0360151b1ad3f754b511065c8a15a40eead0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69040380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7235e70bdf9c275b5ad93b13253b54c9ebc7e9728913bac1c8fcbf39c8a8101`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 10:54:01 GMT
ADD file:8073185e7ca9ded5b755d41c6e6b271ac3eeb13accedefc51935a2ef173aa944 in / 
# Fri, 26 Mar 2021 10:54:07 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 15:48:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:48:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0602fc01f39ffcae884dcb0ce753aa9f918b25b3dbf0527130db85a52ae23c87`  
		Last Modified: Fri, 26 Mar 2021 10:58:00 GMT  
		Size: 53.1 MB (53147418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1644fe478d2fe4baf12ec289cf704ffeae47219f908c0003d9f85b69ba5434a2`  
		Last Modified: Fri, 26 Mar 2021 15:56:09 GMT  
		Size: 5.1 MB (5134178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebd6937ebe551c76ff20b4d4376d63cb8df6517263728ac6c8f13d7bdac6399`  
		Last Modified: Fri, 26 Mar 2021 15:56:10 GMT  
		Size: 10.8 MB (10758784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
