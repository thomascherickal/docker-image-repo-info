## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:b65db8c55226b12456ecd6d0da76e1d9443ceb85a47b884316bdac907b45b02e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fbdd760cedc24102c6086cad1761dea3dd2dcfb578d85c93a04a866d9dba112e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81847163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ed8988fbe6b1f73c58d8e4e755b3205a7e33d5cce745fa5039b5a94c0fb20c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:47:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:47:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:48:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcab7dea4651aac567c69f854a39a4b1812d864e404ee263435f5e8b613f7ae`  
		Last Modified: Fri, 18 Jun 2021 01:06:47 GMT  
		Size: 6.6 MB (6645090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153a310d48b2a006957c2a8a4566c3eacfb84df95abe83a16d2ff807fd4e5c6`  
		Last Modified: Fri, 18 Jun 2021 01:06:47 GMT  
		Size: 3.0 MB (3022967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f79aaaae2ccb877168b7dd5002c60b5f064739ed714229a050f5770e0f80ca4`  
		Last Modified: Fri, 18 Jun 2021 01:07:06 GMT  
		Size: 45.5 MB (45478400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:82716944f3dca77a8be68736a24db88ed1cc826e0667d2fd927c909651a98a64
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71267932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59ad347aba99f48701ad5add622efcbdae1696008152377dcdb64e1da0465a65`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:57:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a5d177b942ffdc4ea1bd38657a5260144a159f44870abb0391ff3b9368cba`  
		Last Modified: Wed, 23 Jun 2021 06:27:58 GMT  
		Size: 5.7 MB (5714727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed17143c1f1eb0fd284d3ef25b30d7ae156670e514aaf64a1b104250774f69`  
		Last Modified: Wed, 23 Jun 2021 06:27:55 GMT  
		Size: 2.6 MB (2584339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc37b4240c27c4c516f976f4b5b9cac3f700b651678e4cfd9aa72b39445673c4`  
		Last Modified: Wed, 23 Jun 2021 06:28:40 GMT  
		Size: 40.7 MB (40671265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6b297c7fc94d353106dbf64276d91f318a691502282d847af6b098c27a4b1573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75863662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bddaceca7a91be06c6458335075a3d77b8c9eab84fcac762cbbdf2f0646bd611`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:14:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:14:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:14:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b4e3d923fc4212f098fe31cf52637b7effa1f210642dde84feacbbda26d639`  
		Last Modified: Fri, 18 Jun 2021 00:22:51 GMT  
		Size: 6.1 MB (6085751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c430f3f1b89b9a2560a61b7fdabaf11e5b6bcfdaaa9a701be61014e5a3544510`  
		Last Modified: Fri, 18 Jun 2021 00:22:50 GMT  
		Size: 2.8 MB (2782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2608e4176c0592850d8ca87f6b172f8d73b159fee3527d2d3648f71fe5d386`  
		Last Modified: Fri, 18 Jun 2021 00:23:10 GMT  
		Size: 43.3 MB (43266792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:44d788212af8e14faefad081f8fe2c94b0514635d27dd2a98e1e8e139cb5e35a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84393818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10277189140070acf0c07d8761a1ba09cca556fec3220245df62196bfc378173`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:47:53 GMT
ADD file:3065820b37abf9a8ea82d39405ed55dc52d1e1ae7591a0a9d1c8a64e7287e06d in / 
# Thu, 17 Jun 2021 23:47:54 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:06:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:06:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:07:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f76fac8c74a781007cb52b5223c59c8f3908bc41ecf0ae8f6dc9046b0aa24e58`  
		Last Modified: Thu, 17 Jun 2021 23:48:46 GMT  
		Size: 27.1 MB (27146196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64eb164cfacb42a07b1981de033a40959c6f45ae88a0548cc8807f50ea78881`  
		Last Modified: Fri, 18 Jun 2021 00:18:06 GMT  
		Size: 6.9 MB (6932635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd10a156118e5a7734c72df779c66591838ec2e31dd4003b207a4b6020c9eb5`  
		Last Modified: Fri, 18 Jun 2021 00:18:05 GMT  
		Size: 3.3 MB (3252100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785110248ac7a9e1554dcd2e0357a0fe0e94369110d15aaaa63bf9a554f0acc0`  
		Last Modified: Fri, 18 Jun 2021 00:18:31 GMT  
		Size: 47.1 MB (47062887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b78372fa64d6f87bc49c4d48a98ebe1e762ccca15b9c657f11bfefbe9d539a0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94916604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d077b2f2fc6071653f71ab5bb86a4f8f59f6df0ac91324e3eb894744a3b07f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Thu, 17 Jun 2021 23:48:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:49:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Jun 2021 23:52:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6adf59f1c1ddfc347ffad19be654c172ca8b7d88788f58f39db9ce0963d623d`  
		Last Modified: Fri, 18 Jun 2021 01:17:13 GMT  
		Size: 7.1 MB (7056303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d3a101e15837a071e560ea8f535c4a7c2bc79b3f14deac5b46931398b7778`  
		Last Modified: Fri, 18 Jun 2021 01:16:57 GMT  
		Size: 3.7 MB (3719555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe694450b2acda0597138d196ae39ffc94fbc3b8b0e8ae1aef2db5db9c4b6b`  
		Last Modified: Fri, 18 Jun 2021 01:18:43 GMT  
		Size: 53.7 MB (53715390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cb2cdd877ec496d30d9aa3dbbc833eae89735e3ec32a912d178cce0a4337e1bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79690828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93b232a16e2096e3578abfe0281c7cce6489e5b717038472f2f1fb2aec0b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:27:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:27:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:27:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3e4792acb448429b177716d4b34b4ff1e2d7a56f6a6331ffba9f76cfb6d1b`  
		Last Modified: Fri, 18 Jun 2021 00:36:30 GMT  
		Size: 6.3 MB (6334310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb995aa1a04a08057e7bb77677374ef1e7a7b075011b43cee1597dc9054140b`  
		Last Modified: Fri, 18 Jun 2021 00:36:30 GMT  
		Size: 3.0 MB (2974902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45a61c3cb40b37fb40fd4173c45d237276af7ced1c9723479e59fea8c86ad84`  
		Last Modified: Fri, 18 Jun 2021 00:36:44 GMT  
		Size: 45.0 MB (45015447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
