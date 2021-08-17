## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:310d9a4a0144db9d3606e2735ed437dc12abb7f4d0d8e8f6c14c7472701f5fc8
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

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2f35c5316b2d555e3ceaf660edb6bf3a5be12499597033debb6260d51c0430a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120106995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261d9f298b8385a12a970d688be20731ac55d600319d1f74484849b8a74843b8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7a7e0c92e8b1915cb1739d97f78556e76e259b9daa2d00ca03131bc457543afe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114792745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e68bc7445db85768887e9e23b0cdf7f2eee73b7efb80dff87a5a9b130fb3ab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:34 GMT
ADD file:4a4158b5432e31cd686b7b2874c22d86a381ac71c3146fe6746501db3d216b41 in / 
# Thu, 22 Jul 2021 00:49:35 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:03:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:03:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 02:04:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd9bc325fb9e2673d4a4f97499e5ac67f82d24eef19ed2cb8d13af9c9256d20c`  
		Last Modified: Thu, 22 Jul 2021 01:01:22 GMT  
		Size: 48.2 MB (48153246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac5ad14f3066e98bd031f59bcd25af51c46975f1f67aa9e984aae49997f855`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 7.4 MB (7376533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538b6814e6bbc64643ef42ffb80c592cecc6833f8c77baa213b7d572de2f060`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 9.7 MB (9687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc7d7506f4cd2a0d1ab64ad0e0a5e9863175a5bcadf61c19a25091d861d34`  
		Last Modified: Thu, 22 Jul 2021 02:21:56 GMT  
		Size: 49.6 MB (49575389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ad644d96ced7329a4fbbdc06340c75993b803a4b0cf007e08531c13da72fe634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913ecee7c9dab2b07b5a7ed95c8d649996bc97a468d1dd89872fdd682edf7bac`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:21:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf69efd3b547fe4dc472fd34a54c466b82ce51b7f04957779206b5ea0ef9160`  
		Last Modified: Thu, 22 Jul 2021 04:41:23 GMT  
		Size: 10.0 MB (9950872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7430ae4c6b93ca669cc72566a38f952b74dece32c5897c46e51a5907bd5a0c`  
		Last Modified: Thu, 22 Jul 2021 04:41:20 GMT  
		Size: 3.9 MB (3921255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5849792410ce49abbe1ff9b523687c9a52997076c1137a38ade9efa2c1e2a2`  
		Last Modified: Thu, 22 Jul 2021 04:42:08 GMT  
		Size: 46.1 MB (46125851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:979207df88c768a50ea4464f7d2e5453c209c86d6bc02435faf36e94b0bfe61e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119068878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a330397b7a843d13fb7c78f8c09c217454dce4f824b8a92d696ad78edf489843`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967a8f1385966af47c9f250997e3158c319d498adc004c91570f770ceac5045a`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 52.2 MB (52167528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8845b954ee6e639a8049d94011685d7527b1332aeb4c3682d09c3c794c330ba3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113280237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06197923c458161f5279e33410b2717bb95576389fc81f281ef3cfb86b73709`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:29 GMT
ADD file:c83a7d581497b7df343b529417c3b904cf901379d5124d738ac2539c778912a3 in / 
# Thu, 22 Jul 2021 00:41:29 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:10:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:10:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27f236654eb1268b8d3986746d9f9fc7ef6d5ea038754025d6953961a088aff0`  
		Last Modified: Thu, 22 Jul 2021 00:49:20 GMT  
		Size: 46.1 MB (46097283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24560580734eb3c4c5331fdde7d8a3d17ba1b35f71b600a58360649f09e6d605`  
		Last Modified: Thu, 22 Jul 2021 04:18:33 GMT  
		Size: 11.4 MB (11352389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b500f684c69eb6ce0ff51c27787bc3252805e441e32a1d1e6b6879f88b8308f`  
		Last Modified: Thu, 22 Jul 2021 04:18:31 GMT  
		Size: 4.6 MB (4564931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac29db6935e2a2be72fe8554711ab48afd994a1424d9cd924579cc424c88cd2`  
		Last Modified: Thu, 22 Jul 2021 04:19:01 GMT  
		Size: 51.3 MB (51265634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7c61d5504630bf2a9e44b82659d9a0922d5ee2a2e52616b3a4969cbfe961128c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117194134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a09736cba9bf334307534d98d213b10913053ace8eec793c120e54981a81885`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:22 GMT
ADD file:1a6aa3d9fc5224e35958d4109d5bcb3afa5948beb85e45b91f46655fe8fadb2f in / 
# Thu, 22 Jul 2021 00:09:23 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:42:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 00:43:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfc6cf8967b24f7ad8c4469c3140cf3967000ae27e3b40b7c72fb89755953841`  
		Last Modified: Thu, 22 Jul 2021 00:15:25 GMT  
		Size: 49.1 MB (49080577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f1ec44468b6cf3c95775fd68ad34176e3f3f5b114e01ef45fda232435a0ee`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 7.3 MB (7252390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5a98fef30417ecbf0d84d2f4e0a5d8c4c745505f4453d9d128eaabe85f0caa`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 10.0 MB (10016296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d36b0ec1b127ef255da5d2ac89935eebf1177a48ee713fa2c190f0357961a9c`  
		Last Modified: Thu, 22 Jul 2021 00:55:01 GMT  
		Size: 50.8 MB (50844871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c1b1e9d990057bcae3e8a85a3c5d12c79353cb674f9f209b94de37a7a11d0bf3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130639799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5a75dbef398dfbc59036490f1073539b586813612d81d577e8abc5458d22c3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:18:15 GMT
ADD file:e6b00a20c003d499ec3793592cb620a450afe5de34f408e897ae9ea6efde50ea in / 
# Thu, 22 Jul 2021 00:18:25 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:04:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:06:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdbf50ea37550aa240918e3856b527a5dcc59fb570024ad98c902fe59e2ffd85`  
		Last Modified: Thu, 22 Jul 2021 00:27:11 GMT  
		Size: 54.2 MB (54182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4eb1cdb7dec331ac914405cf72cda55e246497aa6cdfce759e808d8b0ef32`  
		Last Modified: Thu, 22 Jul 2021 05:13:39 GMT  
		Size: 8.3 MB (8271846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1473db4da98c45802b5d0ee67cc543db64220182999ed71199a61f006246bb4`  
		Last Modified: Thu, 22 Jul 2021 05:13:37 GMT  
		Size: 10.7 MB (10727883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074eb7243d00a87169e9668977de9e6f8c1b4add7e5ee0b9a74e679a90f8abb3`  
		Last Modified: Thu, 22 Jul 2021 05:14:59 GMT  
		Size: 57.5 MB (57457626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a044abeac4fbcc17421729859e0ad8f8146ca185d3f84d7dff789e3fa424e95a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117668556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a5dc7e166298c14f85ce76f7e2ffd7f9ec6475b5b9ba004596a5a9a0b13af6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:21 GMT
ADD file:0862dc2e420958057c0edfbacc39968850751ffdec84962ab8577b7787c5296f in / 
# Thu, 22 Jul 2021 00:42:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:11:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8776c37054ddd28ba8fe526b8dbc08bf7b521ae9ddb8eacd008d05185571cde0`  
		Last Modified: Thu, 22 Jul 2021 00:47:50 GMT  
		Size: 49.0 MB (49003783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c06f635d71fe906f56e25278d5659aa940f095c1ecf199e41436e197534383a`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 7.4 MB (7400582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f57129f34059279bed7373d2b35f16c94df2418b85c5ae20dc715f2e1999498`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 9.9 MB (9883324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f6521600d1dbe8e9e84511427b15a7cb2dd42039504bb9679b6ed7e7ee0dca`  
		Last Modified: Thu, 22 Jul 2021 01:28:00 GMT  
		Size: 51.4 MB (51380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
