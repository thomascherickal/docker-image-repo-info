## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:2c73bde0ad3363b5eea5948e18978c173714a5e7c6aec4ea35c267339358000a
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0b2527a1d3c803622da0cf6458fd628d98b86ed2303abdd8a2cbe442519228ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128541208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56176d9f3db71dd46307d373a6961b91a069aa0b0cbcbc3bf9ce5f55947453f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:57 GMT
ADD file:049a34b0a455f2d6bb7472efc8b4fe28600f9b16fcf86c66e654f0d7f96c617b in / 
# Wed, 26 Jan 2022 01:39:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:10:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:174dc37d1760a198250a591524de55fe80951eb332d1b5fda14aa58b2d0274ae`  
		Last Modified: Wed, 26 Jan 2022 01:45:22 GMT  
		Size: 55.6 MB (55560743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ad4f3c5938976e31cd1193f27047d074e6094f3e599687768b82217ddd84ef`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 5.3 MB (5280293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ef7f4634c596ef4c86e1e87d912ed9ac6798192b66dbec54ebf05b66e5023`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 10.9 MB (10915315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a045598fc6de01a49583f44ade3b3b00e5820b17344162c2fbdea94eb012469a`  
		Last Modified: Wed, 26 Jan 2022 02:21:11 GMT  
		Size: 56.8 MB (56784857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:399795c286656937d53bce1408cdee08cac253682b7c4e69890256caa3823754
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123236656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304a327f049a1fb3837cfa3d8471d796398083dd0ad3b154c0374ce7e5a96214`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:23 GMT
ADD file:2b96a854a3c9d11256be667f9d982d7d8b9dc55dbebd8b4b5fd405cb278a1c64 in / 
# Wed, 26 Jan 2022 01:40:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63d07b82886a825f18700c37fbcff6322772ad2aa7c6337ed53204a0fa13480d`  
		Last Modified: Wed, 26 Jan 2022 01:55:24 GMT  
		Size: 53.0 MB (53020183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786dbbcc14b50d4e55a52a72c123614a491ab523193b076c2c3567fdc1888969`  
		Last Modified: Wed, 26 Jan 2022 02:51:24 GMT  
		Size: 5.2 MB (5182484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1bb97567a73aef32ddc428fed052ca711f5df4a1975daa855a68c2d3ce1ae`  
		Last Modified: Wed, 26 Jan 2022 02:51:26 GMT  
		Size: 10.6 MB (10582661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba482fdbbd02271877b484e0ea6a914eeb789145001e985ecb8effcc2fe524d`  
		Last Modified: Wed, 26 Jan 2022 02:52:19 GMT  
		Size: 54.5 MB (54451328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cb44f8ee191d3a9392ed7c2e9d11f2d19c95aad22f1ce6278f2613f346c8376c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118255430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de53e4b6a787226c8de580b8b40bec33b13304a91de1efda17e1e6c98df657bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:29 GMT
ADD file:0d5c36134a34929922dcd5c83256b9539a94c46d5b7dcd23ae6cc29721bdc320 in / 
# Wed, 26 Jan 2022 01:40:30 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:34:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9276ec53f1a5aac51c0a8a27bcc855b50a696f144903a4c1dfab1a458f7f7af0`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 50.7 MB (50662778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faba8178fd562af6ed1b6193d73a2eefb5dbc9bc34e5e155d0b644f8d23281a`  
		Last Modified: Wed, 26 Jan 2022 17:00:54 GMT  
		Size: 5.0 MB (5040739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de84da60e6b5c715dc34fc6124ae223b3288b8777242a15fdfb7dd0d91a9261`  
		Last Modified: Wed, 26 Jan 2022 17:00:56 GMT  
		Size: 10.2 MB (10241353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3548f7f03a19175e426fc70dd9fcd2f355f5cc861cbc242716094aa8d3f704d9`  
		Last Modified: Wed, 26 Jan 2022 17:01:39 GMT  
		Size: 52.3 MB (52310560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0270af015615b24f4b5bc2742541d00bf62db4ed504b9248bb8608f8b92f5963
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127306774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b08eb6db757ade88d2b4b3c57b0afd27c90daf15da918b974c1dc31889409f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:585d9a04ed59d36d1ee8be3ad5a7a488962b12f0b7d737826e25a7ab617521fe in / 
# Wed, 26 Jan 2022 01:41:53 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f9f8cc8e22fa2c53a109b770bcaab20fb907dd9957eb312d9f49000ff4185f8c`  
		Last Modified: Wed, 26 Jan 2022 01:47:52 GMT  
		Size: 54.5 MB (54535243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8a0926c8b86f048958ba5be5355985e20305f2a6df3fd52b867ac3cfcb7ee`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 5.3 MB (5269783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7042a90d872d1ef29a580051968c7437ef7f8f185841fa2ddf3e7bf37bb0593`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 10.7 MB (10676573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7233b23063ef3fe482c0973a9442a36485028dadbd3cb2d8bf3bb8269274f7`  
		Last Modified: Wed, 26 Jan 2022 02:22:58 GMT  
		Size: 56.8 MB (56825175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:46260cab74918eca54501375c1edf30cd915040fa27d308a99be23624be5a51d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131519438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb0e917e3ea3bf288fc252c80f0d34abf67a31ed7ceab0114fa218e781512f4f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:06 GMT
ADD file:49bb0653fde7eea7609e6ad9bea8c405d8a514818936cff57f87f5fa321d2582 in / 
# Wed, 26 Jan 2022 01:39:06 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1308dabb988bd1e94f15ca40572eaddec8a0de059ca7c28b6a83e6821441d6f8`  
		Last Modified: Wed, 26 Jan 2022 01:47:24 GMT  
		Size: 56.6 MB (56598143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7ba5a7115e901688cba13f3ffc91e6ab2cedb7a7cff304d4bbb5606c507f4`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 5.4 MB (5412384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7645e93b83f1c523ab6c715a08bbfd71c80611ee830755b1e36db82d26c1eb2`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 11.3 MB (11307381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b85a21b4a33dd378fe3c4484dab108da9bbae3464368991728734991ec15143`  
		Last Modified: Wed, 26 Jan 2022 02:27:11 GMT  
		Size: 58.2 MB (58201530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:aceb972971590e61b669eef950493d1f324ce9dd66cfb2a4ad9accc71f9d949b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125997048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d9a5416f38edd45c703c01b5355680f3da0a50cfdd0d02d693a16c9a6f95e8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:27 GMT
ADD file:cb994d31e0dc06b73ce5e197fffe27837867fce8ab87a858b9668290c97bd7af in / 
# Wed, 26 Jan 2022 01:41:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45126d37a1c34eefb327242a121bbca1be988e1e2e1cf037fde7eaa131fd6db7`  
		Last Modified: Wed, 26 Jan 2022 01:49:20 GMT  
		Size: 54.3 MB (54262039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9463250f8710e43e5aff116a08f617cbc14f10997bd69f2bda7a81f002b2e7`  
		Last Modified: Wed, 26 Jan 2022 02:34:27 GMT  
		Size: 5.2 MB (5235335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20371ca4b02d263c2ebdd04847579505ac45245b979462f3374b0acdda280fb2`  
		Last Modified: Wed, 26 Jan 2022 02:34:29 GMT  
		Size: 10.9 MB (10874712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4c2df8a803e41441178f5ffe30f7ee30d91807c496750ff0cae99fc163063c`  
		Last Modified: Wed, 26 Jan 2022 02:35:20 GMT  
		Size: 55.6 MB (55624962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a33bad7823dc6e3edb675834f086d8eae635b559e9d7e63d4764b2a11965d124
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138648953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beba77e6b3deca6cc0ab0cbcac14ad894f2ba7ae49565536520ac00aa1f593b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:815d918aa7e03d3a0e2d0dd87d7d9696feb37b5054d103e1ac83847b08e877a2 in / 
# Wed, 26 Jan 2022 01:45:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fe2b17ea8278b5a905731f1d003664a61c7774f4a23cda61a596487a1b51210`  
		Last Modified: Wed, 26 Jan 2022 01:54:29 GMT  
		Size: 59.9 MB (59942176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4cbdc2b57b1d5abc56a5ce2448279d438e672ad3740a30808c6aca777b1ba7`  
		Last Modified: Wed, 26 Jan 2022 03:13:11 GMT  
		Size: 5.5 MB (5544663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46175642455b8055d9ddc0cbcac8518413ed6ae29f42a87871058a9c7df76e08`  
		Last Modified: Wed, 26 Jan 2022 03:13:14 GMT  
		Size: 11.7 MB (11693166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2209b60fdeff528905267562368c5bb713edc81a5b929e3c31387a9f3cb62a6`  
		Last Modified: Wed, 26 Jan 2022 03:14:10 GMT  
		Size: 61.5 MB (61468948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d4a00ee5dd1d59d8ce995a893ba66ed74a43040c6c0412d11db8ff661c1549cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126059871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3462214aa9f6799b0f41aa247c4489fcd3a4a00c880adfaef58bb1cae152bb00`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:21 GMT
ADD file:b56123b23454cb9db7a2a2e19c5219cf5643b8692bc247ac4212732f2a8d218a in / 
# Wed, 26 Jan 2022 01:40:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:06:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:06:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:06:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4155c67ca83ba1ee87acdfb0ff7b262e769e0a27829b9b44ca097c4ba1e29ea4`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 53.8 MB (53837097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610ffbd8c4fbe8756d41005ec7da9c699f84722392728547ac79401b01064e8`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 5.3 MB (5259010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed15a8cf3570b9b0ddac9365776ad36a5024968df38f3bef0cabb5d6a953eb`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 10.8 MB (10806960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dea4fec3c6c14a2719bb370e7430d7fa93a34e49038af8e8f1e2c0e5ad8d7c`  
		Last Modified: Wed, 26 Jan 2022 02:17:23 GMT  
		Size: 56.2 MB (56156804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
