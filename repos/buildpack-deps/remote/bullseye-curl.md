## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:f0bc68399bc76e1d562de8399f0fb2990e3bd6cc04aab46bb2eb6d789905caef
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cb9a3f7bd43628db1b3695a6e7b28d561bf4df306ab1f63a0c232397690bf2dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71086032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e2c1abde86fb7ff272adfa86162471d1bfa52060a0dec82087fecebdcb31e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4307444787732144220d75296f55023fa4114b856df149c28e78559c50359d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68193987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39186554e8bc668aa17c37b50cd6803d4a408a41ad404ba37b3e10e2ed96267`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:19 GMT
ADD file:b314b98654e8532fd10a08a172ea5c3edb7d7a36c7faf85d06d14be12f7b83ef in / 
# Tue, 25 Oct 2022 03:06:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:12:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1f0ecb08923b99bef3f82c2e88603bb53e3ed084c13252275c05039cc279c158`  
		Last Modified: Tue, 25 Oct 2022 03:11:15 GMT  
		Size: 52.5 MB (52547473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b399c5eb53b4c35fa33682a82d73bdc4b096cd78ae95fe36c4ed81d18f6849`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 5.1 MB (5072235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccdd06393cd3873a3cc8b9cbe170a2032fd61d1d545b7045b649faf2f4e732`  
		Last Modified: Tue, 25 Oct 2022 06:19:02 GMT  
		Size: 10.6 MB (10574279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fa161c8e7935e0810bcd3ca45a9746cf6e3fdc6025c5362e8bc2648f7fae6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65358325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86ef37d02c678f38add592f5f88e1f266a851783e8f323eb1837a5ee7352ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc7e9978ee6d44bb721af5cba9e40ee69de8d269140ec556a0c40cbeee8979bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69727646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b9fd10ad56e7d5bac1e3cb67021a7765c589e6e7d144f46d1c76d2811413d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf477637cd09b9031cd034fff22d013e90a3101df053d80729d928601fb7c14a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72143373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4b083b9d9929246daf9a5fe0622f9a1e88bfb618b352807b23b97d75ff5a38`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:19 GMT
ADD file:aa26f69b37c3e144d08e17bb9be7302ec89ae0579121c874a35f336d7077fd3b in / 
# Tue, 25 Oct 2022 02:22:19 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8caf426a2703f99fb0be4b03411ecaa580d102f7c47ef43b422b6d7c13c380e2`  
		Last Modified: Tue, 25 Oct 2022 02:27:54 GMT  
		Size: 56.0 MB (56023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b92a2ff5c72653a0679aa7f5e2bc695011c0a71faa424229e560957d204dab`  
		Last Modified: Tue, 25 Oct 2022 05:27:37 GMT  
		Size: 5.1 MB (5086887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6856a3002e686ceb6d48d078731366f576ed3adcb73bd49dcb300057732904`  
		Last Modified: Tue, 25 Oct 2022 05:27:38 GMT  
		Size: 11.0 MB (11032526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:668f750c6d59a65e45714ebe9fd3c02e2b07e166cf39df660a4b93a59449e9ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68845705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e70040762c35b1ea015572f262495cddda025b3d915f9fbfa15e0a0f6b02130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:469e7517e99c19831cea091b8ba496389124880b75d31d2718cc6c1999060b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75961034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cb6ede5f74b2e5a7f231d8ef2d1f5728c8b419020b8d7640b6aaef3bdfe00e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:28 GMT
ADD file:c01a6cc4222fbeeda5c2d679c5b355539880a02c792c64861eb17b81a3678f45 in / 
# Tue, 25 Oct 2022 03:13:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:14:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ee5a342763ed1d31bef8cebe9f4cc5dd6d427f630da679a87da0427be7b22e3d`  
		Last Modified: Tue, 25 Oct 2022 03:18:52 GMT  
		Size: 58.9 MB (58916374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a4727f39cbcb19b39abdbd847eeceed842ef65f8514372024c48b913bc951a`  
		Last Modified: Tue, 25 Oct 2022 06:49:00 GMT  
		Size: 5.4 MB (5414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe601e6c8a1ec9c69c49c65a53339202a65cea9d4f01d161fb34905c06a4a99`  
		Last Modified: Tue, 25 Oct 2022 06:49:01 GMT  
		Size: 11.6 MB (11630153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:809d9d381f46cf97b2154255bf1ab72c6c7126ca14bef3939630abde9638783d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cce275c18bfdc19a1e7f27773751920f1a720c0ccd64c54a8ace1b33e0cf31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:31:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e8478a953d3a464d73e36e4032c979725bc79ce0eeb83aca30212de549b90`  
		Last Modified: Tue, 25 Oct 2022 02:49:32 GMT  
		Size: 5.1 MB (5148477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdbee45ed722bfaf7e9ba90503afa7a0cf17b87fc1bfa1e87cbf49ca6bd7d9`  
		Last Modified: Tue, 25 Oct 2022 02:49:33 GMT  
		Size: 10.8 MB (10766704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
