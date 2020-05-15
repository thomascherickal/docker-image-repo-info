## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:1e446f483f053631bb50bb83a7b5a12513e307001016b94706b964812e6adf17
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a9b765dd181d64a6985a1ed71c5fee86c28db96afef89c30d15d05fadb37572f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125447056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b95a2edfd395d61a0305388cd3cc37c26733cc22631e1c7b3ad46766b9c264e`
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
# Fri, 15 May 2020 17:31:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:19105d4e0710b44c9c203f25e1cd393cfadb8e9d1b33855aa6641533d625c4f7`  
		Last Modified: Fri, 15 May 2020 17:47:30 GMT  
		Size: 55.7 MB (55658572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4f87960b1b9ff0a791046e9705fdd767ed1c6ac5ee0f95da399cdca3f2ded871
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120326790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6e1273ce97c533dc8b71b1484057f072e0532a9d067e4a41e6a91a232dec14`
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
# Fri, 15 May 2020 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:19fa5c09a3e017a2b7a2b6e53f1c3afa3978189e8bbe966b83cfc29251b56616`  
		Last Modified: Fri, 15 May 2020 04:00:47 GMT  
		Size: 53.3 MB (53295430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cb0fda9963a2a8f5004f222f90377fc7f42325e9c0caa30089ac7dc2734e3816
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115303764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996c9f9c223696533c3a1211660fccd3d694bd2042e653c57e59545588acae02`
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
# Fri, 15 May 2020 10:30:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b15989d6fd8c30478f6d030c5c9aa82929f5467d22588698401d7bed07a35e74`  
		Last Modified: Fri, 15 May 2020 10:56:22 GMT  
		Size: 51.1 MB (51080530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c35df4a2635394b4dd4876e48ff35e61e8d62d251d9fde5e7a5e5aeb57314fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124400769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:289449ac44a4fb30b37696fa8ad656d3acbfdb2e61144e27d8a5e2a948ea9379`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:52 GMT
ADD file:642f1f8b3928c38913b91b5770e5ef77e0467db31d0e7342848c66b97b0cefce in / 
# Wed, 13 May 2020 21:41:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:19:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:19:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da14fdea4bf7eaa36b82ecde9ee461379c7eb32fac279c7d1bce1452edd5bf2f`  
		Last Modified: Wed, 13 May 2020 21:52:10 GMT  
		Size: 50.3 MB (50328349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d18f3d952fdbc982edca77fab71409bebc6a0b410a5f13ffe6fd2685b6020c`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 7.8 MB (7809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382abc5b67b7c0e46916f728a90e7aa0866070c3a67e581de6b5904092e6ca45`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 10.5 MB (10459917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30ad6c82e2b7a536da67a837bec581308704d1e15eaf6e92c24578b56e187d9`  
		Last Modified: Wed, 13 May 2020 22:38:32 GMT  
		Size: 55.8 MB (55803040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46b0d06fbac8424ea20d736b576514a257850bd7edbacce3fe74f89de96c1444
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128952727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0623ce93af14919a23fced5900f602ae59d86b227ab15fdb51da6335245fbcf`
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
# Fri, 15 May 2020 17:05:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a629d631fe32949e213eb3eea28481d067b67bc40e33f20f2bddd5076a09c189`  
		Last Modified: Fri, 15 May 2020 17:25:30 GMT  
		Size: 57.5 MB (57518069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7f740990a60a29318bd72ad55ff0b6cc352e5ebd341c12b1719ff40f4cbf35e3
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122673838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100ba60ecc8b9228351d64e0dfdfa83b15d17a6c2aaff0fc88302a1057e30213`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:47:32 GMT
ADD file:f2d8d152f2c12223430241ba470d074182fc4071fbe07696ef9a7ac73d7e31c8 in / 
# Wed, 13 May 2020 22:47:33 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:50:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:51:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9fe8ffba560af94cfc9c2199a294b5143a198e0cbe44469cb586e1986f063ea`  
		Last Modified: Wed, 13 May 2020 22:55:41 GMT  
		Size: 50.1 MB (50131081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0640353f1b9db4814a57a569a8417ac7dca26baae0a3342a2575bad188f9e2d`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 7.5 MB (7460937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce2184377077db50bd5cfbf56505a742cce1db802c2fa42946c103a34a61969`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 10.5 MB (10484779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648af14339d9e6a970776b9e7d360437621c1a759c25c603b49426eb0a234705`  
		Last Modified: Thu, 14 May 2020 00:13:18 GMT  
		Size: 54.6 MB (54597041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3a7be10ad2e88263a6697ccb41ce2f072ab2af20392db6e434af2459ef7c9dd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135693870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76abf0378f9c85f53029205aac12168521ef58f6ecc2c0c1eec5cbd9e1e1cc5`
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
# Wed, 13 May 2020 23:32:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f12dd448830e6ab4491686ac42b85cc8f50e9b182a8b19722842140e7e06c1af`  
		Last Modified: Thu, 14 May 2020 00:25:53 GMT  
		Size: 61.0 MB (61049897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a37fa2451f22e1faf623ff758c49cbc31126238581c2dd450459fd708f0b887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122850865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e1cc32ef5ad64b06b71e6636d87ce8c1f780322974a279a6035e0da14d481`
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
# Fri, 15 May 2020 04:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:775b4e20d2d0e51cbdce841c11938b1192f017a82d06190796de1bbfabcc12bf`  
		Last Modified: Fri, 15 May 2020 05:08:08 GMT  
		Size: 54.9 MB (54899878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
