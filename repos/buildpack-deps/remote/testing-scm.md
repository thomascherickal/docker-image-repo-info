## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:4bfcf0784b0f1a69585094b199e407213c5ff09f3914eb3535980c4f8d1ccbb5
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
$ docker pull buildpack-deps@sha256:3ae2c5e2db053973615a7e69d31cb620e271d0aab33be1eb2874503af3180b1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126044229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eddbc89710efa94f2c7d1bfdbf8a7b5f4dc85d299f7e5d8293b33dddd29d30c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:09 GMT
ADD file:730ef8e3327df644cd47994a561a489bfcce5da8103cc8eb34e67321a36df2ba in / 
# Tue, 12 Jan 2021 00:32:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:55:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:56:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b802c2c29a7757c7475a0b343a18a46b6b27dde9e3fb6b4db61c68ea197b51d2`  
		Last Modified: Tue, 12 Jan 2021 00:38:04 GMT  
		Size: 53.6 MB (53566443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd06bfac0a19b28c6511794acccc260657d53a299701a82ec9fcafe465089350`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 8.0 MB (7974792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d97704dcad5e05944cbac93df8fdf452cb71e698fd44004184391a44e8787c`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 10.6 MB (10649126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782396cc8dbffc61d005f86b48ba6f88b4dbeb6e71f98f909b15d1e290bc9273`  
		Last Modified: Tue, 12 Jan 2021 04:04:59 GMT  
		Size: 53.9 MB (53853868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c15af854bfab268f82ca3d2e9c7f146d4eaeb356c273d9c903649f4e47c3ccf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120900925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4db8d3ba0d55ba24701a1d5dc598f7ab0418dc2f63ce58038aa3c32eac28e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:50:29 GMT
ADD file:d4da31b3c934d9b6c8328e7951f06cec1babe1f9674a7a3ee2e87670575ff01c in / 
# Tue, 12 Jan 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:24:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f9810833d48e3d19cbfbfb8871ba282d104d5bcfae1b19c0c003f9811dbe7c4c`  
		Last Modified: Tue, 12 Jan 2021 00:58:53 GMT  
		Size: 51.5 MB (51487444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257fe5697f52f59aa0dbdede36db8adf4c0796905b3388832de43ac1e4ab97d`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 7.5 MB (7527914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59bb7c72bcd7ff3df84ab37209a928574816146c37f0808619c4b5a6dde4a1`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 10.3 MB (10335674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2064b7463d16bbcc2e8bc6d085c083e4e8d5bf88ac7a254843dc12449eaec623`  
		Last Modified: Tue, 12 Jan 2021 01:42:15 GMT  
		Size: 51.5 MB (51549893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f4b9b04a7fd7f1b0f928cf77727d22ccee6d0d57fb667dc6df2a936debbe63a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115986961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f620c32dff17f0d7ec48eae47c6736f2ab35b896baa806ca88473ab84b8c4f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 11 Jan 2021 23:59:52 GMT
ADD file:ad9ce4dd05291eba636daae5f0b9de510927734ac26dcca6940d93e88b5c5330 in / 
# Mon, 11 Jan 2021 23:59:54 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecb0a075e68a9a1a4b7394123b05b2811afa9bc0a23170e2e6c42d5ee19a7ac`  
		Last Modified: Tue, 12 Jan 2021 00:09:56 GMT  
		Size: 49.2 MB (49159573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dea32ec53c55b5a19d9fb093241be9ba6e2fe2fd55963111e57d39b0973f01c`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 7.3 MB (7265094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b285ad78deb9119d75d41a2decc62fd9676078225d860eec32d20835fa7fb`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 10.0 MB (9975049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e47a7484b9800c33e8812962a70ed0114c8572b070a16230fbfcd1c09b7a60`  
		Last Modified: Tue, 12 Jan 2021 01:28:31 GMT  
		Size: 49.6 MB (49587245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f705e8da66d1b18bc506306b59c7c636bd6977d6876864aadde391e51081d67b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124885421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bc8b71d4e0ba06c6a85cbe9d8895348408a99f518c344e652e1e281d04a6913`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:49 GMT
ADD file:0700c58361c6ae34d399d7ca2a5a6f509980a496c07d319f7455d86b483e7f25 in / 
# Tue, 12 Jan 2021 00:39:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:19:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:20:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1e62204d5e176f9e5ef453b346203f7bda9e22ed810a0a4e2c14548d7cc3afe`  
		Last Modified: Tue, 12 Jan 2021 00:50:17 GMT  
		Size: 52.4 MB (52428437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f37b86a934fe39fb5aebaff30977af7d0075b2eeb06b1b794582ae2566dff1`  
		Last Modified: Tue, 12 Jan 2021 01:36:53 GMT  
		Size: 7.8 MB (7840062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ecaa573834d3855dd61a0aabaf6565245ab200624d87774802a93f1b2dea`  
		Last Modified: Tue, 12 Jan 2021 01:36:54 GMT  
		Size: 10.7 MB (10654799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b5a3d04882a1f9723afda0d32fb1325ffa21fe435e1088c0b1736b2ba28cc`  
		Last Modified: Tue, 12 Jan 2021 01:37:17 GMT  
		Size: 54.0 MB (53962123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8198f65498bfef730ebadf77e507fe6e9ed27aee9ad83aa0e38b6dafca690f84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128964466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5ddd5c02f860a22451ee9f84ad0ef1a7e3eab68da062e6bce20f4649af8666`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:38:50 GMT
ADD file:5bf2c8336f63e88ae7e3d1d6804439d7f6a54937823f8e72b84f8bc95c97391e in / 
# Tue, 12 Jan 2021 00:38:50 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:15:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:15:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a8d8d38d6122a88724bab503447c48e782190ba13d75634b2b651e6dbe0a0225`  
		Last Modified: Tue, 12 Jan 2021 00:45:03 GMT  
		Size: 54.6 MB (54617930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c3a2f57bfbcccfb355c377855cb08176af609e0a121945636c2af1f19b110`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 8.2 MB (8157573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e0211a7714f69b0754581dbc4d3b367733f5113d0b6a49c72623b3327621b4`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 11.0 MB (11032217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e630fdae63dfc10347058d61bc56b367781b3c5d80f350c52f780f10c94a1d3`  
		Last Modified: Tue, 12 Jan 2021 03:30:07 GMT  
		Size: 55.2 MB (55156746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:56d4931020e10192c4ab53943bb3c361eed3ca6ef8fec6f752e6449d37d3c03a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f89edcacfff36bae31e8201f95bfb5cd1ca653f5171baefebf219250a59d0d57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:15:12 GMT
ADD file:171276d9060030f06df201450c4356d6449f4c6a905d02db7f2371f7ed26b34d in / 
# Tue, 12 Jan 2021 01:15:13 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:45:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:46:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cdc62d8dca2f8e7c324fa9f4efc40193ada4c98be9ca6b3f1388ad903e4bd5d9`  
		Last Modified: Tue, 12 Jan 2021 01:20:56 GMT  
		Size: 52.3 MB (52264790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b87fc90acd9bd7359cfb81de768ce7f4cdc0821db3ed523142fe855433832`  
		Last Modified: Tue, 12 Jan 2021 01:58:49 GMT  
		Size: 7.5 MB (7492735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6084ef3498948096f602b4aac1a0fb7a2dbaa7d5d751897ddec139d2cebb08f`  
		Last Modified: Tue, 12 Jan 2021 01:58:51 GMT  
		Size: 10.7 MB (10657326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d002bf71507be6bd90480c0b53df54edfde519a712016ceb3e562397e7259f42`  
		Last Modified: Tue, 12 Jan 2021 01:59:44 GMT  
		Size: 52.6 MB (52588286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:18fc66fbef60f5e267c1160af5ece96bfdf7fce4ae82c914002d27858cdb78a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135551510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a472f4fd09304780a49cca6eef9150a327b4f52964041baaa23204f3fc33866f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:23:03 GMT
ADD file:840490bff9a0b2cb1e20599d893c1160f6884327f51294479567e5d43f91b885 in / 
# Tue, 12 Jan 2021 00:23:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:39:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d21ce86f5496c36ba2ba289acb977a3b160c6c56fb257c10e3adb8b55164a16`  
		Last Modified: Tue, 12 Jan 2021 00:32:24 GMT  
		Size: 57.6 MB (57562164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42b61558772eb59064c0ebad8029e0e7524bf865c29218b048871cd3e43fe7`  
		Last Modified: Tue, 12 Jan 2021 02:37:14 GMT  
		Size: 8.4 MB (8431230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663cfe2e2cfc28477e509f0e7aaffd4159d2f37157b32a7327bb6f43a7508ac4`  
		Last Modified: Tue, 12 Jan 2021 02:37:17 GMT  
		Size: 11.4 MB (11421868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe449d18af822c075f40a6ecd99422667906a91875941e650eb90b9743412ec4`  
		Last Modified: Tue, 12 Jan 2021 02:37:47 GMT  
		Size: 58.1 MB (58136248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0a1f052510f4b6448b50eb2508ed41972565ac1a1c5645668c0e5c24e4dfafe3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123610720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80b1b376f93e52cf93a87169d292e319ae42f40974bfc0489d6dd9c4f35461f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:41 GMT
ADD file:5007beabc318acc6a33d879e231105324ef7801fb709d3d69813b180e883d64f in / 
# Tue, 12 Jan 2021 00:41:44 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:07:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f1b527eede6bdcb4cce85e897c3a92fbf04bb476403758d3b535dbf6e388d192`  
		Last Modified: Tue, 12 Jan 2021 00:45:27 GMT  
		Size: 52.1 MB (52107904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f7f4dc3450e7b31e01a1746ba85df290d5b698d495c8ab448923393956e52c`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 7.6 MB (7649499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945c37e35656a95430c56e2a6bb0a416252a37130eca65d1f3beee38efee696e`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 10.5 MB (10525963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7df15c7e29c90193fbc5bf8d91410b9860ebc7c3975d2951c83c543f5cef88`  
		Last Modified: Tue, 12 Jan 2021 02:17:45 GMT  
		Size: 53.3 MB (53327354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
