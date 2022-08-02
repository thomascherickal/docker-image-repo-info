## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:29c2121c8869c80f80d43c9bf39cfcb18554359b4df863fefbf5760ed74f4f53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fae035187641a69b1cb1b10a20dddfca6c18ee078c72127d2d5d2909a0e1465f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131436527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f47b81f1dc938c0ad7246c0429639cb3046133ce55c098bcf02f871b4d9395`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:52 GMT
ADD file:8f3d1b2e7474fdc04cd1135312dce29db677e5567ff094e59c8338f5bd2465c5 in / 
# Tue, 02 Aug 2022 01:20:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:50:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:180517453f08358cf15a4972d7eafc4c2c649be2333940572c68856727b63bdc`  
		Last Modified: Tue, 02 Aug 2022 01:25:57 GMT  
		Size: 53.2 MB (53231560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea3bb192fc1a2203afc9f801c7c8a19b9753282603b3c8a634578bb887beef`  
		Last Modified: Tue, 02 Aug 2022 02:20:42 GMT  
		Size: 9.3 MB (9305398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd36f037efbbab2cd1fcf04b9f87ba901b2835ba77678dbf9521f200b225fadf`  
		Last Modified: Tue, 02 Aug 2022 02:20:42 GMT  
		Size: 11.3 MB (11272509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6e842d076eedbe41a37a67ac7ad354edf3b5ce4a0b2c1f76ec89f7380d6bfc`  
		Last Modified: Tue, 02 Aug 2022 02:21:00 GMT  
		Size: 57.6 MB (57627060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7898539069871fcc91cdb4cceda9570567bc9b523428de6882445a6d4e42ae60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127096678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:492f0b2ced30ba4bfa6eda150cd97683bd1046e1aee31157aadd60df1bf55919`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:23 GMT
ADD file:2829a8dbc1e67454e67c0015efaaceadaa4b04330ed9e60cc8248246cac2aae2 in / 
# Tue, 02 Aug 2022 00:50:23 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:25:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:25:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a67d4cf31e6e9dc8797a5c01d3198f326d91410c372d1a490bf5592578d9b1`  
		Last Modified: Tue, 02 Aug 2022 00:58:37 GMT  
		Size: 52.0 MB (52021372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6833771528bea1307d56591db306804d9768947a466a60b5de4f6b545ab0cec5`  
		Last Modified: Tue, 02 Aug 2022 01:33:35 GMT  
		Size: 8.7 MB (8741294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2288f8703c485a4ea82b9d9a1de8905ae4f0e420ca4f317625f441977a31c0`  
		Last Modified: Tue, 02 Aug 2022 01:33:34 GMT  
		Size: 10.9 MB (10946981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd5022e5328c139a6024dd9522e3ee6548067f8bf3200154271988ebb0457e`  
		Last Modified: Tue, 02 Aug 2022 01:34:01 GMT  
		Size: 55.4 MB (55387031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d8c512d64ae9ad3f2e481314f1d4855e30a77f85dfb63a640eb6ff02b4a5ff41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122110023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6687a2444cb5290af981f96b82b906a1625d2f8c7971813168b9f6add445c97d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:00:45 GMT
ADD file:a1d27fd37cd41b3026c10df50adfd5a93a40194548a87a372c97149f63b096b3 in / 
# Tue, 02 Aug 2022 01:00:46 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:51:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23e34b183a37464e321571d2a75fa33fded0e5a8506066db5c4f20153a665c2c`  
		Last Modified: Tue, 02 Aug 2022 01:09:03 GMT  
		Size: 49.7 MB (49735351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50b5c584586bbf2589138734167dd8e14560e75cd854cd9bca75019a3f530b`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 8.4 MB (8423017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4818fead9ad7b4ed572aa86d08f341272cc2cbb418cbe22f7f7d71f2be3778d`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 10.6 MB (10589650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd163d2eebe4936202350772d43aa0c00eba5ca32eca150d0f23e01feae220c5`  
		Last Modified: Tue, 02 Aug 2022 02:12:28 GMT  
		Size: 53.4 MB (53362005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:63bf85ae860dbf4528de20d612dcc51c333e01dbb9abf1e5f3cf536ab2505a52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131233972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c8f4017b6299569189621efc421ec9f3ac8e6bcc68451b7e7451f86bc84b3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:27:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:27:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:27:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e49dab65b12b89c427063ea6eec0802e14801664648c428e5a774754f3e73`  
		Last Modified: Tue, 02 Aug 2022 01:47:00 GMT  
		Size: 9.2 MB (9150009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b71a9f562c782f5916aedb7846293c7057b9f5f32ac072f785d2b21839f530`  
		Last Modified: Tue, 02 Aug 2022 01:46:57 GMT  
		Size: 11.1 MB (11062337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205e62166cd9b96a2220ead9f68603c3996816c0b7e279fe1afb47d74ea5975`  
		Last Modified: Tue, 02 Aug 2022 01:47:20 GMT  
		Size: 57.7 MB (57709839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c3cd94d46ccad8d58831e83863795fe9c80f9d8aa2da3e331ddc8dffa5443b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134262167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fd7be2d65fdb87669228ac919618bb59c6320e34d1af2bb2e129b587f4c47c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:12:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4385d16696693ee42b7a7f20009fa801f71ca0c6e014ce30f294f40d9993e965`  
		Last Modified: Tue, 02 Aug 2022 01:26:51 GMT  
		Size: 9.5 MB (9480230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed00b31a2aacbca3fdd1dfb26c6e14bf0bfbd4ab13f2498063fe7786ad715669`  
		Last Modified: Tue, 02 Aug 2022 01:26:50 GMT  
		Size: 11.5 MB (11473533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd03748d20b403da16ec2105506ec777552bb9d8960f48500514674a687d5b8`  
		Last Modified: Tue, 02 Aug 2022 01:27:13 GMT  
		Size: 59.1 MB (59113338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9f2e0633fd097c4b93d54591e6b739d66101b1fa75c18976ddcfd887dc5fbc95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129290133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43beb762e9b16618775de009b9e28cb2bbb96bfed3b221c499f5075eb1ce7810`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:13:16 GMT
ADD file:6165703835b4dbffafda027e272e21bf37cfc276085814fa1d03c1db0162e605 in / 
# Tue, 02 Aug 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:13:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71112f7b4dfd928d54aaa23ee1023fef50d2dc747bf6e2168afe69932ce8aa1a`  
		Last Modified: Tue, 02 Aug 2022 01:24:23 GMT  
		Size: 53.3 MB (53305987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523353756f561bdc5914e25ea1cfeda5bc330e894285664b88d8ce11aa594a29`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 8.7 MB (8659688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2258650534e83b3efae8fb3f1ce269322b09b63e553775a7c0b8c8104b2451b0`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 11.0 MB (11041802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e365e2051b826228522cde5e4dc082e794b8ccbcf39513ac4bb385212b6277`  
		Last Modified: Tue, 02 Aug 2022 02:31:24 GMT  
		Size: 56.3 MB (56282656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6123c5ad7fa3716831ca5a739061ba89d728ec9f55210bf5e5423b131e251274
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141679433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f202865500436ef2096d89c6ec75ca84e8126a7b08c32a799b55e8b78531a958`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:27:28 GMT
ADD file:8039654bddce2cd83d9433d1df0a53c329e7877cc8210593bcde23de63e2f1fd in / 
# Tue, 12 Jul 2022 01:27:36 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:49:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:49:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:50:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0d4394941206b4f218ffa2a2b794698da5149ab7a22b52f71390aec65a7add3e`  
		Last Modified: Tue, 12 Jul 2022 01:40:47 GMT  
		Size: 57.4 MB (57441462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e13dc094f3be3cdae228630277f198c2aee4ccf4989e03df692829782575ad`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 9.9 MB (9889588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9148c549699d52333ba063274d8397af520c8317b8d893c23ba0800047eb2b45`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 12.1 MB (12082932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c97a942b806632ce20c77655f33f494e860c5c99b3cbbe88c8a6d4a5eda5577`  
		Last Modified: Tue, 26 Jul 2022 23:51:54 GMT  
		Size: 62.3 MB (62265451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a554d40bdf614dfd9e405a249dbfe2bff02cb93429ca042ff9db3c8e0b1c3124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122419082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eef1028664b4597959820e5ea3724c58b7a5eff1763e4f7d9729c7729d13014`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:11:50 GMT
ADD file:e156d172727c94dd7b17970577469d9b556db67960762f454d5b90dad3f746bb in / 
# Thu, 23 Jun 2022 01:11:53 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:59:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 02:04:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70334332338a08f7ae515b43812936d5898e62e8ffd5fd38ba59761c5ed137d9`  
		Last Modified: Thu, 23 Jun 2022 01:30:12 GMT  
		Size: 49.4 MB (49429796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5fc26886e551b626bc82f99096f4659ee9ee5af689dad0d03fc75d88c37d88`  
		Last Modified: Thu, 23 Jun 2022 02:51:42 GMT  
		Size: 8.4 MB (8394795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6176147b43ca0f721514815cbe526cd0e19723ed30c23a9a3534a95d32d19cb`  
		Last Modified: Thu, 23 Jun 2022 02:51:43 GMT  
		Size: 10.7 MB (10650389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebc8d66990654882c5fa423a1a4c713b77656fe3fb7540e4e51bbfcd8395d3`  
		Last Modified: Thu, 23 Jun 2022 02:54:14 GMT  
		Size: 53.9 MB (53944102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1b28e370b7f14e632e1233e966d5ee08666aaf6b5ba3db430f74ab03e9e0325a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128798317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0683e4467933de232d93780c8cba1dfb4f123ec25ecec0298b98c61c8eeb3dbf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:36 GMT
ADD file:19dee33de85aac92620de3bd92768833a889db0b60b7445419bccb4285c46f94 in / 
# Tue, 02 Aug 2022 00:43:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:12:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:12:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31888e988211ae2cd4058438d0fd3d3420a26d35f21e97741527c1e85ad2d476`  
		Last Modified: Tue, 02 Aug 2022 00:49:29 GMT  
		Size: 51.7 MB (51734666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd60a4351ebe5fad9f32c09d0a6f7ec29b6c6dcb5ff8c29e6650149557447e2`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 9.0 MB (8960873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440b0db795ce4385e2a159326c7d9ab52e109942607b82b1c377894e874e601d`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 11.2 MB (11166864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6891cb8548d01d5cd140a6d90fa3462f4433c9891f74f6d5405b9556edaca1a0`  
		Last Modified: Tue, 02 Aug 2022 01:37:13 GMT  
		Size: 56.9 MB (56935914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
