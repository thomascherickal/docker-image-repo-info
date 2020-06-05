## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:9dbc349795ffa8107f72f83379f334bd9edc0968985aaeed49604d9f89883566
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1046fb013168bcfc2b210056123e58c5c69cde8b9db49bb1f5a4f7fe0f85f841
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69788484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e371fc42e20fbce361681c6d5bc4ef359d74e974ba20c82108070358bdcf6bb1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:27:09 GMT
ADD file:3feae44a900d0e1e835d12f1ea607313fe008d55842495a8cc533e7cfa75064f in / 
# Fri, 15 May 2020 06:27:09 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:30:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5acaaf333e788954dc63603194f262baba7644709169c9584c92237472fe3a9a`  
		Last Modified: Fri, 15 May 2020 06:36:49 GMT  
		Size: 51.4 MB (51391128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86454c7eb0ea041d8338f7821ab10f9501b14d3021a4d5f2dce05ba946d9188`  
		Last Modified: Fri, 15 May 2020 17:47:09 GMT  
		Size: 7.9 MB (7934302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd76374a13b2aafe8574e44d4bb42e142c3abe4fe7b7f1f82ce19cdad51311`  
		Last Modified: Fri, 15 May 2020 17:47:09 GMT  
		Size: 10.5 MB (10463054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fe3d0c4c775b38db477323f0745b0d9a4c0afdbf53b4e80987fe365d81a73715
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67031360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c6ca734fab60ea981e67aa1392ee7da511f7e157d32db62c99929ceb9f7b64`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:36:28 GMT
ADD file:099743a0547d5c892b4a3daaa3fc0f05d8317cd4946a0e9508d130ee56db63bb in / 
# Thu, 14 May 2020 22:36:31 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:38:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:38:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0238daf30887e241cdd1334fa6bd5883d06738c7ff61cea1b32a3361de098564`  
		Last Modified: Thu, 14 May 2020 22:45:51 GMT  
		Size: 49.4 MB (49359451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f1dbc2de2b0cbdbc9ae5411e2efb20958587e0c8691a15a5755669fe35e467`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 7.5 MB (7514224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4b62e0336252e727cea159b040a0ef9263bc7ec15d9411459056795050f87`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 10.2 MB (10157685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9a1f0c1f552e4694f0fa3cd2d95a8734270749b420e2d9756de0d42c3b0eb0d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64223234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d341a769ad7240b4e5a0fa46c3f85f65d96748ddd305e06c950e53122b0bee2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 00:58:28 GMT
ADD file:c0d2fe9468c0056452ba2eba677a3cfb1318edf3174c0106a65ec1c5608f130f in / 
# Fri, 15 May 2020 00:58:30 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:28:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:29:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:add59fdfc3a148d6f3bc80c671fa82b62aebfbe6f2ed783df08b083fb9497d23`  
		Last Modified: Fri, 15 May 2020 01:10:22 GMT  
		Size: 47.2 MB (47161514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed350c74909d45b8bbadbed0841a0212e60d10edb4e0fc351433b86807c174`  
		Last Modified: Fri, 15 May 2020 10:55:58 GMT  
		Size: 7.3 MB (7256985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0fe0276714c46bcc2d93dd77955362fe60814e5ec6b075e68a97b34da7f34`  
		Last Modified: Fri, 15 May 2020 10:55:59 GMT  
		Size: 9.8 MB (9804735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eb402da809b044d5ed1f2bcbf45f0a62d1906e7dfb7c0b8fe820ef37e056ff7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68598288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d087b070933c93310e6e1fd97062dfecf1defc95fdd79e5f3c10259ea70f609`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:41:55 GMT
ADD file:47e352caa545ab1122a3a9df6a86296796c3b1633a1a8151d6fb438f88b47d5d in / 
# Fri, 15 May 2020 12:41:58 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:02:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:02:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:523842c45f03b461bd15f8ec65b3e2670cde3c595006ef67af2d46f30e971812`  
		Last Modified: Fri, 15 May 2020 12:52:36 GMT  
		Size: 50.3 MB (50328985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e57198818fd11918588ce78d9cd056305b237e52e37463ed090e08379da0ff`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 7.8 MB (7809462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a6e14baacb6f567947c7991213c158c4924519e3e8e989752bb8ff12813c7`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 10.5 MB (10459841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:16aba335f3ecc9ba7d200ca0f016e51b35d0e57a61a264e6cb280a2b8458d3bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71434658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fddb901720aa77f56446b2061a8093d37e9bdfc64117f93fc70a7e2a79dfd2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:06:18 GMT
ADD file:7290df675cbf34dadbbbb441b1c875c896d0027e51ef4f0322ea750d256dc1d7 in / 
# Fri, 15 May 2020 07:06:18 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:05:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:05:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c978edbcc0f43d7a702a8796ed2e5dd9443fd302b396d9b20d4472b6152672f8`  
		Last Modified: Fri, 15 May 2020 07:16:58 GMT  
		Size: 52.5 MB (52481343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51518769fedac128b59ec5b081ca9002aa4c0af29f5a7a0c8ec1b3d02d8c4bbb`  
		Last Modified: Fri, 15 May 2020 17:25:02 GMT  
		Size: 8.1 MB (8112069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e20b512a546a13c02057a9f7978b41d29d8e7c70a91f8c2d9d6b09db8f5c1e`  
		Last Modified: Fri, 15 May 2020 17:25:07 GMT  
		Size: 10.8 MB (10841246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:93d592500d66b6133edd7399dc473e4c5566519d11fea7f6abae1b0acf42226b
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68098079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26f04112c16877a017d8bb147f9222e5de20bfc8cfc19dabf077ef3d1a77ee3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:46:53 GMT
ADD file:fcf688b002e58dbfd2392e8a30b0ad1975c59c068b68c9d846430ce0f63eb390 in / 
# Fri, 15 May 2020 04:46:54 GMT
CMD ["bash"]
# Fri, 05 Jun 2020 21:38:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 21:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dcbeba28f7aa4ae28ec4e38f90ddc68bb34f71bf49e3361203df2f569876774f`  
		Last Modified: Fri, 15 May 2020 04:55:03 GMT  
		Size: 50.1 MB (50131847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d0ed8dc6e716f36dc92c5111b99ac84ac31e108fa46c6a77978317ff5c8d6`  
		Last Modified: Fri, 05 Jun 2020 21:44:34 GMT  
		Size: 7.5 MB (7460933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a86a877eb6ead7b0031c439d2b52cdad0273b54b9dfdf91f3106609216b07be`  
		Last Modified: Fri, 05 Jun 2020 21:44:34 GMT  
		Size: 10.5 MB (10505299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ff96ccb1581f10a5e5b2c8aac3e45cddd4e477165af7a593e003ef4f70e5ee1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74643973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed75f631222c95416bf21fac81e046bcf15366c944806a08b7a22de54ddfa6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e43969f6c0ff55aa4240214980deed196b68292106e0144d8d1290495d9b7`  
		Last Modified: Thu, 14 May 2020 00:25:02 GMT  
		Size: 8.4 MB (8356860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eacce9e1d274d8f139e9d384ceb5e66a86ca1857d025523765b1b099330719b`  
		Last Modified: Thu, 14 May 2020 00:24:57 GMT  
		Size: 11.2 MB (11176806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a45df0c708c032a0d468804feb0bc736655c9535d8c8caa52f5524cf7f30531d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67950987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79054d0eea77f9cb5c6984e0dec031e24d11e204cf3e30430879de98cd58e1ef`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:05:50 GMT
ADD file:56a2d8bf46ec4edd3d768966ad8e9b4c86561cbcd482ae49fc18cc34306d54fb in / 
# Thu, 14 May 2020 23:05:53 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:58:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f0cbd757e4d594cf3793c18e1f7d5d6f3fd983ea05bd2edeac4774c47e85b763`  
		Last Modified: Thu, 14 May 2020 23:10:41 GMT  
		Size: 50.0 MB (50002620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb69a5809930b7b8812ae832cb600c60afe5387c53903bf422ae0e80ff086583`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 7.6 MB (7600625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd25c680ce576408f8c9a5e8891ea37ac21483e932a4bacc4b744cad80a975e`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 10.3 MB (10347742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
