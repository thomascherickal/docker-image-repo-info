## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:f594123d1e875ddc7d1a0dee8c2ad2d615d45e5feb7d750470e6f897b02306d2
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
$ docker pull buildpack-deps@sha256:fdb9d7a53c26b540bb3d3bb095dd0762a80eb878d68407c8d93cea9a250064c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128966171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea216e0704122a3376d318b4dbfe25be09c97b629c32c753af40f1c5ff5f320`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:21:48 GMT
ADD file:084dc3db6641669bf09de94b7a32f3180ca32152a22a677961428ad78324f10c in / 
# Tue, 29 Mar 2022 00:21:48 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:28:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:28:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:28:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6673186ed4ed62930866783fb71f9386d0ece250e264d269d06e238753c30392`  
		Last Modified: Tue, 29 Mar 2022 00:26:08 GMT  
		Size: 55.6 MB (55584323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df04644801f7943b709f58330bcc6bb7f022f170144d520e3ed86de27038730`  
		Last Modified: Tue, 29 Mar 2022 17:36:58 GMT  
		Size: 5.3 MB (5268987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faed9fc4a14be51a64a07e3c2c778a51e2c2d8fbf4f7f4e4502991884520e0a5`  
		Last Modified: Tue, 29 Mar 2022 17:36:58 GMT  
		Size: 10.9 MB (10923809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774237b19b51c64e2dec4de20d289c9fa3ea436c5c9ebca3c443d811e7ddf0a`  
		Last Modified: Tue, 29 Mar 2022 17:37:17 GMT  
		Size: 57.2 MB (57189052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:bb7f5c46626d12381975d367b143219edf2203af090efcb0c68b3db1d72f886f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123565854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb50557e3713520235216ce35aab735bafc92f342a1927d468deccd32bbc2b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:07 GMT
ADD file:6b5b5c095508b777a2c8b2633d97d6143bfab0320bed58e8e335179bfd681fc9 in / 
# Tue, 29 Mar 2022 00:49:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:38:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:39:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b209f6efb315c2c09d16e50d6077a10a401191c741a83c3c6c0767fe202d69d`  
		Last Modified: Tue, 29 Mar 2022 01:03:30 GMT  
		Size: 53.0 MB (52995524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc9d490149e4bcb11fe298e2c5a923c08cc31f08662f9f7637aca6473309b73`  
		Last Modified: Tue, 29 Mar 2022 08:02:54 GMT  
		Size: 5.2 MB (5163931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132e128b11ccea17e38c248a34ec3142776903dcca038a3e7789c9e8f52f6a1`  
		Last Modified: Tue, 29 Mar 2022 08:02:56 GMT  
		Size: 10.6 MB (10597029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bea4cefcae02c237fe7371ca4d568c1f51b28d10f874dfcdd78ad48b4b5234f`  
		Last Modified: Tue, 29 Mar 2022 08:03:39 GMT  
		Size: 54.8 MB (54809370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:66bae13fab412347a2cbfb241f5efc782ae483eab0ef04602c7f2c56ab69a114
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119096156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc57abffc4609497efa38a7ebb3d2388189066f8a44fdbabf5f73731b87e504`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:29:27 GMT
ADD file:819f7eacc6077672fc50aade09ce96ce0ef1e2b4d9bd84e706ea22d90d73799a in / 
# Thu, 17 Mar 2022 09:29:28 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:48:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 02:50:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fca9c92eb5afd37d0b08a4fba4dd30ea576686d945af655ae46133854768127`  
		Last Modified: Thu, 17 Mar 2022 09:44:45 GMT  
		Size: 50.8 MB (50761706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5383ea443f2740a52246a5eee4a417a2b1244a1f912208d4c96428520670a4`  
		Last Modified: Sat, 19 Mar 2022 03:26:13 GMT  
		Size: 5.0 MB (5030714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d3f50feb52a7829302a09f9e4f362e90c5b18f7be314c43c43c6b1cbb89dea`  
		Last Modified: Sat, 19 Mar 2022 03:26:14 GMT  
		Size: 10.5 MB (10475768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66566945e25367a4d188cff5f444e5c148cf8c32c44b9a8b417c7c6950ce026`  
		Last Modified: Sat, 19 Mar 2022 03:27:01 GMT  
		Size: 52.8 MB (52827968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e79fd6e582dd3bee124595ff9ceb3871bfc347948c837b226a1c1fde284498a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127668580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cd5951072478c2a639ae53ad5c431cf05c207b5a275e856bd3f03a98bf9aff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:37 GMT
ADD file:8a0795f999cb36975538f6060cde3753f8d82b0c997ba2861ab1e317b5dd52a1 in / 
# Tue, 29 Mar 2022 00:42:38 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:11:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8fa507a56d88ff151c2943292a587b9de276f98f32670b4a39659e57e5f891f6`  
		Last Modified: Tue, 29 Mar 2022 00:48:52 GMT  
		Size: 54.5 MB (54505175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5124965babcf0efb0b9f697d0229a02548fc8e77f38e8a3318f5476392f0044`  
		Last Modified: Wed, 30 Mar 2022 02:23:04 GMT  
		Size: 5.3 MB (5255023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7db0732ad45ae55988f8c7a467ee60a149ed5e30bef581b352b4ef3e0a51fb0`  
		Last Modified: Wed, 30 Mar 2022 02:23:05 GMT  
		Size: 10.7 MB (10692742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c00599d7e87d8d24f989cdf597ea5c119384bb9b61e1a034ba1f80b2d81370`  
		Last Modified: Wed, 30 Mar 2022 02:23:24 GMT  
		Size: 57.2 MB (57215640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7e7f4df6480567258d5bdbd4f7a72bbe07a707af36338964e6ae0e39615fe3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131744957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d38e772feb103d65506c709d2a96069d476b1bb7becdc4177965fd44cd85b9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:20 GMT
ADD file:828aa883b729cb9e3bbc9efef043626425a2803461bd7b07862d746e2df08c10 in / 
# Tue, 29 Mar 2022 00:41:21 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e0acfe1e9e31a265994eee72788e1a0b4b33edc5c9d6fc978fd65d87aa94b53`  
		Last Modified: Tue, 29 Mar 2022 00:47:47 GMT  
		Size: 56.6 MB (56628219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1b01718568970f8976ea798ed333d8acb22b4cdc57a341b078bb0a7e4e4dc`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 5.4 MB (5400088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296971f2bacc0edb451554653b20751f9adfa0cbce82cb5e06a78c72076b036a`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 11.1 MB (11103529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f03b11aedb9bbc81a6111cf72e7c011c9682d79ce42ad6dba4bac5f1a2340`  
		Last Modified: Tue, 29 Mar 2022 18:14:03 GMT  
		Size: 58.6 MB (58613121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b8fee69864b233a92ed8b6d5822a190fa190cfe5632e646f47ad57f1ae989978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126085794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e672d1ede339aba1da7ceb30c333dd3b1a868d93299b70e01fa0f2ff4f96b09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:40:39 GMT
ADD file:88e75745fdbfd0784c1c18134a0a52a5534df18201a6f49555a5c618b4531804 in / 
# Tue, 29 Mar 2022 07:40:44 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:17:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bdc3f4c024aea887030bcf477ee808da6aa3e6683fb111845d94ab4f2480ff24`  
		Last Modified: Tue, 29 Mar 2022 07:50:58 GMT  
		Size: 54.2 MB (54240334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e94f68f0d96094b4bd1aa9ba6f4465ec7d6879ed28f910b949ffb165eef3fe`  
		Last Modified: Tue, 29 Mar 2022 08:54:21 GMT  
		Size: 5.2 MB (5221857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd581c56a027feec68bb7a881cac731bca045297cd76398414512c34351a063d`  
		Last Modified: Tue, 29 Mar 2022 08:54:24 GMT  
		Size: 10.7 MB (10672471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631eb84b5e85d4e37526f1ae6b1259a7a43e8e02c45f72f851783117629e90a`  
		Last Modified: Tue, 29 Mar 2022 08:55:13 GMT  
		Size: 56.0 MB (55951132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0053bed0b7a1e1761cb1fee867ed996db25d9904be642887e9f2dd3d1d4f06c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139113055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5155314e54075e4a93b0f43156dc592225d511d363017c2b4162b88121bed87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:20:10 GMT
ADD file:c9ff325b9fe680d344c36e7e25729f90711bdf646908892ebdc0f3a53d92bc50 in / 
# Tue, 29 Mar 2022 00:20:29 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:32:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 05:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc5522fc3ca5c5e9e4af133a35ed8a4e104c9366b7ab66c3cc5601aef68f175a`  
		Last Modified: Tue, 29 Mar 2022 00:30:15 GMT  
		Size: 60.0 MB (59999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31127088a5022a99c9c420931875f462b30887ac8cdd2b9832e9a48833053641`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 5.5 MB (5543257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20e81de5da1931ed0a987d558ca1844e91b01be66fe4fa9f9a11ab9c2e851f7`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 11.7 MB (11702051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9353b28a9fb4647d78b62d393fd6fe5b2983eee962f4429ab69b8baedb393997`  
		Last Modified: Wed, 30 Mar 2022 06:24:21 GMT  
		Size: 61.9 MB (61868324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:37305a789a3733ebe0b8150df0204f5d8bc3b689a8bac40fd4858f460d8b7464
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126462957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02bcac061e8afd5b333d1b4d067667873e79da6df5df79de20694d5b33fd111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:05 GMT
ADD file:9a99e896abdfac4163e20511778572abbec89bf317a3c3dad1f6fe0c63b126b1 in / 
# Tue, 29 Mar 2022 00:51:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:23:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:23:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c231abb22533340c714e28363f98b83f5da88a6702fdfc7d06ed65b8f2e70e1`  
		Last Modified: Tue, 29 Mar 2022 00:57:13 GMT  
		Size: 53.8 MB (53839067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1f72f77effa39a86785d5e5242154a329664927615884293ae53de3228e345`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 5.2 MB (5245181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40794a51d7ee7ef5a9c0175be5b9245646cf0f2703acbb34ea8e72c731272f5`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 10.8 MB (10819318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c986ac3bb53ec5a4892c250c435a3e59ee79ddb71f265aa5d083d3f87a1faf3b`  
		Last Modified: Wed, 30 Mar 2022 02:33:07 GMT  
		Size: 56.6 MB (56559391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
