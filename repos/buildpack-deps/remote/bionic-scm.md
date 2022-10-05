## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:9f2ae4f96815fd625fc2bff014865882882d05fbed41be15ec027bf4207dcf05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2185d9b019c2c7ffa24811155449345078f4adb96a6b771140d25fa96128e80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81864921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18c1737a8adb0820fe73beb358791cbde70dc5a532a61b2fa74b072d928cca6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c135384e7b3dd71613cf28fbeb9805b51ae11140898b2d9034275ce1c7c77988
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25e3b88b9f8e85d32a18eda77ceaf66170755d464f812b3b79a2aeb16210730`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:63e2e4107976dcdcf6ae6988bd8ee7890d04668976081de5baf582fa95a9fd5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75673809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f69480af9b266f0e8fef34454b654f94eb6135333ae9654ac45e3d0e4d064c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:27:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:27:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aed76b50c469f7d6d0bf1c162cc5a083b434d904ab7c5f0812b615ecb01fa76`  
		Last Modified: Wed, 05 Oct 2022 00:40:54 GMT  
		Size: 6.1 MB (6072093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff78fce69652894d1a72406000210d4504f8533af1a699d691ead64173c61f81`  
		Last Modified: Wed, 05 Oct 2022 00:40:54 GMT  
		Size: 2.6 MB (2571161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee012fdb2017d6c7c5ba08057db06e166b5f370cb25382979273b94324255ae5`  
		Last Modified: Wed, 05 Oct 2022 00:41:12 GMT  
		Size: 43.3 MB (43295961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:566ce652bb82f95743ed4c98395ff3f418fb4479b396063a7d451dea9ca2af1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84208214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7959aa272c3c45292ccadf93386acc91eebc6638f12188773edaafea930f776e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:51:15 GMT
ADD file:ee35e95b906b98c2d7493d8c365bf5aaf351251abce763f9be2d9fa6cc541aaf in / 
# Tue, 04 Oct 2022 23:51:15 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:15:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:16:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d1a231d13b300fc73c20f074f3accd74dcff41afd006c272719fdf8cf9be075`  
		Last Modified: Tue, 04 Oct 2022 23:52:01 GMT  
		Size: 27.2 MB (27165243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3870bdaaada14e54f8f8d9eb057687e0bfb87c1fe903c4e8e92c9e67beaf1470`  
		Last Modified: Wed, 05 Oct 2022 00:25:24 GMT  
		Size: 6.9 MB (6919671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9580368a218667ca55403824a289d3e9c10b38535dfbf28f861c91bd10f95cad`  
		Last Modified: Wed, 05 Oct 2022 00:25:23 GMT  
		Size: 3.0 MB (3039920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98ca390f0b9413df5c623843c331ead702b47b4dde8802132e72fd5c9df94a8`  
		Last Modified: Wed, 05 Oct 2022 00:25:42 GMT  
		Size: 47.1 MB (47083380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fc7d7718c22aef1838fe789a1e10b2769eef4ffac7c13c46bfba6ddcddc9ab6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94957028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe392debaed81378c54884166ab756e786f56dbaede35409e316b0c4fda09403`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:48:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 18:49:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc281606eca5927568a33babcc79e53b7c86b8b366758571a82800859c9d2775`  
		Last Modified: Wed, 05 Oct 2022 19:16:11 GMT  
		Size: 7.1 MB (7050115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c346db0a167811b858cfd4e45644384e1f0c9f32224229504e7c34c554e0558`  
		Last Modified: Wed, 05 Oct 2022 19:16:09 GMT  
		Size: 3.7 MB (3720178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee93c7799aca3cbe9af24c9787a6b7eaf1f23e42ca6022f824cd4fe0ce3034`  
		Last Modified: Wed, 05 Oct 2022 19:16:37 GMT  
		Size: 53.7 MB (53744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6cc9153a290d6121b15d9a0f9127162b9c939c8c42758c35b83f975685574119
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79716169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:061199c9320dc4967ab97f5fcd4684b897584b8581a56074dc50989ab2dd39c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:31 GMT
ADD file:29c2a2a72a634a5f21c2f37cfd38da282528b75f75124d04e56a2f86f2e64121 in / 
# Tue, 04 Oct 2022 23:52:34 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:14:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:14:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f41c9e2df5b8fcd28b58de30866b751466a2cbad7eb8f43e02d799439fb377cf`  
		Last Modified: Tue, 04 Oct 2022 23:54:09 GMT  
		Size: 25.4 MB (25370644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c5a6c94d91734296d7e96fa87ac18e5a63bfc1ea10cb69fa156a57e98b6af9`  
		Last Modified: Wed, 05 Oct 2022 00:34:00 GMT  
		Size: 6.3 MB (6324310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dfb4db24bd32706235fb661c35a4ccf9a225e1c0b4fbe33eff8635953c51e3`  
		Last Modified: Wed, 05 Oct 2022 00:34:00 GMT  
		Size: 3.0 MB (2977245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6358485ea5e8f04c0ef04ed033e2b73991c5e7eedb3cd1f37db1742ffe75f364`  
		Last Modified: Wed, 05 Oct 2022 00:34:14 GMT  
		Size: 45.0 MB (45043970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
