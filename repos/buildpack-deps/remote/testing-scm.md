## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:f57e52295202b2c53a2e0890f314f3f0e7d3ced8c3a0e827f41ce0cb6c8e151e
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
$ docker pull buildpack-deps@sha256:dfff17c4317c954868c77bfbbe97680d7a0671789464e3dcf45d7fe05eb7fdd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124785647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8771905bfeb983a2f7362dda3b3f6741c1d8eec4ed4d5ebae7e3ab244a98361`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:24 GMT
ADD file:fa865518757ef9e0af03796e7abd6cbfd59e20f5ae325422e41524615051a2d1 in / 
# Tue, 17 Nov 2020 20:20:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d004aa4da82e9e47169ac4cccf33df9b52bef6dda8aa5f7b0bcb03af34078173`  
		Last Modified: Tue, 17 Nov 2020 20:26:32 GMT  
		Size: 55.6 MB (55578105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5514b41a34cf855f2908da965f01f2b0f68fc62b29b9fb67811a07e7c61d16`  
		Last Modified: Wed, 18 Nov 2020 00:47:23 GMT  
		Size: 5.1 MB (5063216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3985bf4e3bf68c52363fd7853ecc6142b55501eb8457558d27ae10a0358e8907`  
		Last Modified: Wed, 18 Nov 2020 00:47:24 GMT  
		Size: 10.6 MB (10645972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f00fbcbbd3c3783e061ff8d861834c157f06601ed495383250dabb36682027`  
		Last Modified: Wed, 18 Nov 2020 00:47:43 GMT  
		Size: 53.5 MB (53498354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:819824241690c30dcf2ca875edcf5924558b76e50162e76467e9d688ba9f24e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119772978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f782fa82a6fff7ddde87aeefc1fbd8f23bb475efb07350e11d6776fdb76418`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:15 GMT
ADD file:1825c9ae9f20eb2576f772d68892699ef4ca90dff36b8f247bf78ce04ad41a91 in / 
# Tue, 17 Nov 2020 20:19:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:35:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:35:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:36:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8172f634b664f563947e1ba480d8a7e04acd125ff144bde0dabb4ef26db6d3b1`  
		Last Modified: Tue, 17 Nov 2020 20:29:25 GMT  
		Size: 53.2 MB (53174409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9bcac9e1b17a227267b364ec33a309b567898a11a1049896dfb513508befa`  
		Last Modified: Tue, 17 Nov 2020 22:05:34 GMT  
		Size: 5.0 MB (4974569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af90ca1b550dfe775778350f5133681fd06314fe43ae77642bada174068cdcf`  
		Last Modified: Tue, 17 Nov 2020 22:05:35 GMT  
		Size: 10.3 MB (10331991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b1d8db5b8210961e24b26bc3d718e185f5af3264a1eed9a03e56f5f21aaea`  
		Last Modified: Tue, 17 Nov 2020 22:06:02 GMT  
		Size: 51.3 MB (51292009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5fda91a195f0ccf29c27a4bd6b50029255762d95685364a231a0f8f4a1d33ecd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114866261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a8b7ed6cb6851d0b584d47281f5d458fd6388fa51bf514b840eb3f1fcfff61`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:26 GMT
ADD file:f2393813e8311e27cf255e78079f523184619c1ee8ff9ccdf51a5cbc61751e1b in / 
# Tue, 17 Nov 2020 20:19:29 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:36:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:907906fd9e2e517e45080a90701520c1c3c654647630763a4cd9f181ae039252`  
		Last Modified: Tue, 17 Nov 2020 20:30:29 GMT  
		Size: 50.8 MB (50756959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a164f19b5f5e429261a5effb8cbcbbe66d7f6da9e93d9ff34b86f08ed6a42`  
		Last Modified: Tue, 17 Nov 2020 22:04:14 GMT  
		Size: 4.8 MB (4838545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d419d3ef4e0a73ebe3cf3ced0bfa50e1e9961d81ecb60e542323b9bc441e6d`  
		Last Modified: Tue, 17 Nov 2020 22:04:15 GMT  
		Size: 10.0 MB (9971053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb56c58816ba83f360d684e04fd465ae4514e3f503575978543166b4671d81a`  
		Last Modified: Tue, 17 Nov 2020 22:04:40 GMT  
		Size: 49.3 MB (49299704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ec8c805e804face54e02e0c706b563be8024584a92f5a8a6027dd8e38b03aacb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123642431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6f4d56db5489fc7cbba023ce812204f87aaa24b3bc731e106ade1251fe7197`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:22:08 GMT
ADD file:58908becb64a88c580fc5d9fea54a7e73507d1e537e70b5567f5d58c26ad000d in / 
# Tue, 17 Nov 2020 20:22:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df1866c47e1fa1c26619e32544732be4853c6b58bfe5ea76c192ae970daf5da7`  
		Last Modified: Tue, 17 Nov 2020 20:30:56 GMT  
		Size: 54.3 MB (54323419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71907b4dd26e793f4e9841e590a1a930f7265a02f7c07e57767ef9cbe91f8b`  
		Last Modified: Tue, 17 Nov 2020 22:33:52 GMT  
		Size: 5.1 MB (5055744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2cf86d1130240ba8633c0151d4a4a4b9e6a251bf8ec2bf14d72ce40a67727c`  
		Last Modified: Tue, 17 Nov 2020 22:33:53 GMT  
		Size: 10.6 MB (10648270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c6056c2ca2fb8c36f5f80c875444bbf38dab5bc7ebf358fd257bac133169fb`  
		Last Modified: Tue, 17 Nov 2020 22:34:20 GMT  
		Size: 53.6 MB (53614998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:112273b5796141d07de61def08f0ed046485c72266e3d2e98a0f2cc1a62f740d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127762353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da19a817a8d76b76bd6d6be3370876afac4eb49838e404ae319c22a60f7343ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:01 GMT
ADD file:df88ece8f6b35ea6811921d958952eb8431b76449597cb6d5151e88c62167964 in / 
# Tue, 17 Nov 2020 20:19:01 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:01:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:01:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:02:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9137c9a05e5bbf8d80413499157abbe788cac975a7926ded72bd9ff285f7520`  
		Last Modified: Tue, 17 Nov 2020 20:25:46 GMT  
		Size: 56.7 MB (56728874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd9994454c4b84708c2d9754f396aac9f662a7169c2322418210f8d161ac4d`  
		Last Modified: Tue, 17 Nov 2020 21:22:12 GMT  
		Size: 5.2 MB (5182817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87786a5db1b57a9ac7c14addd518c4d55f9ac878f951e8110866257d83d6d82c`  
		Last Modified: Tue, 17 Nov 2020 21:22:13 GMT  
		Size: 11.0 MB (11022570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88de8fd349f0d1c859351edc10905c5adca2e975f84e43d737a1933c7ee86944`  
		Last Modified: Tue, 17 Nov 2020 21:22:35 GMT  
		Size: 54.8 MB (54828092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:43c7a90e58ca2143a232227ef3748d4909c9e360b6ffcb4d11019f8aed73250b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121881063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0388293bb4ddfb8dcccb21c62b12b07b45b3f06f5d47baaf2c4a4feacb8037`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:02 GMT
ADD file:b3efb0da03cf858a9bc305dec420c5a2fd85b3ba7212cd26f4012b931492bcc2 in / 
# Tue, 17 Nov 2020 20:18:03 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:34:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:35:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b53392aabcbd30c0ebb343f6223dffd1e0d3a034f1683d60ac80a65254522359`  
		Last Modified: Tue, 17 Nov 2020 20:24:23 GMT  
		Size: 53.9 MB (53861718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58b5272c361da3f94922fc2e154b2c7092b6abb657a2857ef7684f41294c60e`  
		Last Modified: Tue, 17 Nov 2020 22:48:33 GMT  
		Size: 5.0 MB (5025865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03528b3943b7f8558ee96ae85f7871910f47c9b5f5e89e078ae6da0783a2ff3`  
		Last Modified: Tue, 17 Nov 2020 22:48:36 GMT  
		Size: 10.7 MB (10652787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948afd46ba6a632c8ebf47f170254ed3eeb087a1f06b0ae45b1d02b59145894f`  
		Last Modified: Tue, 17 Nov 2020 22:49:27 GMT  
		Size: 52.3 MB (52340693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1984964e17e3ef966ed20d15d138d40fdd47262a7998ca5385f31015be67ef1d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140915006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6317753d08034742ca5a4e5bb9fdf084dde48dfe95332aa141e4fe15a8dfbe06`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:36:17 GMT
ADD file:29c9502df00306ab143f7a4895ecbd5188710e18fa501d1931dfffe0d2281c6f in / 
# Tue, 13 Oct 2020 01:36:23 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:45:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 08:47:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e449e1f1ecdd90acbe5e4ea9a9f941aa8dcee06a83eb2eff72fe4dd55cc20576`  
		Last Modified: Tue, 13 Oct 2020 01:47:12 GMT  
		Size: 56.5 MB (56486527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b868bd306c5ff6ba6bbe52fb1cc3deaa47fed5a1362d135d89cfca87a684e4a4`  
		Last Modified: Tue, 13 Oct 2020 09:29:49 GMT  
		Size: 8.3 MB (8307201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca5bd324b7e56f3121bd85c3a06132da98d95654678c2a01b4439cab8adc5b5`  
		Last Modified: Tue, 13 Oct 2020 09:29:49 GMT  
		Size: 11.4 MB (11392086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26769c811da7971c25f9fab265e60dd509f2c8522ff89eea05deda913a34b33`  
		Last Modified: Tue, 13 Oct 2020 09:31:06 GMT  
		Size: 64.7 MB (64729192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fd4b8cb0ce6891b62fb90ed9391d24e4ce0987ab6e81fb0f70dfa113b102e695
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122339605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d3247595cd989d1ae99b506fcf1f12e5b3020652ebb0616aa1831916c2a42ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:17:06 GMT
ADD file:b2aa936914932ddd337990ffdd06ceff2628d7198e962be967a9781efaba51d9 in / 
# Tue, 17 Nov 2020 20:17:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:25:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:25:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:069a0f569bbab3514d40a8e2575a33e70926c0aeacc9099b083427a84cafc126`  
		Last Modified: Tue, 17 Nov 2020 20:22:44 GMT  
		Size: 53.8 MB (53806147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0c6c52e6336a9fffb0f96f9bb643f4f181052948188c1e0453ed3ab253217`  
		Last Modified: Tue, 17 Nov 2020 21:43:23 GMT  
		Size: 5.0 MB (5048357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce85daf872edba752735571ddb26859c12b6e958818465881a345aa93faeef1`  
		Last Modified: Tue, 17 Nov 2020 21:43:23 GMT  
		Size: 10.5 MB (10514397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecce1269b139cf68c0820b2ca3d17dcb95e08de624942ba2d3b6512f98f009e`  
		Last Modified: Tue, 17 Nov 2020 21:44:43 GMT  
		Size: 53.0 MB (52970704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
