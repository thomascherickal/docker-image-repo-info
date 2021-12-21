## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:258a786dab0e988188ea848e20bfb303390b0aa7727ffbb15c28d7e9b650c9e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fa9fd8b1bcf50ba6ae239f82ff37e95b7575f71f98224cfbfd103afc330fc52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110787854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04ee51ca350a8c82804e8e8a6269ea97c0d565ce4d9b4f4303ab48954b94e2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:56:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737a610bfddaa0e7c87d11580b07707489348ac0fb4cdf2f2265ff2e60246c1b`  
		Last Modified: Tue, 21 Dec 2021 02:05:16 GMT  
		Size: 49.8 MB (49762204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fbf588a92cde2e8687dfbe8ef8363dc4351ddae620e469ed0504158c09fac145
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106589675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119de5497a77d7e42de837ee815ac9ba1636c994c1701dbd9ee95c5c6a9286bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:57:10 GMT
ADD file:a2c8513298faf10e5f3b6a070d46acca10a79d9dd50302c55604df9fecb26b2a in / 
# Thu, 02 Dec 2021 02:57:11 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bd29eaaacb1755f329ce7db7d99eb138c06aad3ab1bb6e8c3b0017596eb1f69`  
		Last Modified: Thu, 02 Dec 2021 03:15:21 GMT  
		Size: 44.1 MB (44091702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e812372186481b18e85105bf8f717c7b3462bcd83b7cbd968f30acebe2349d`  
		Last Modified: Thu, 02 Dec 2021 04:06:51 GMT  
		Size: 10.4 MB (10352021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0272bf1fb82e41a2bd28b3fed21300f54f34aaade421e0b2a669c53136a0d8f`  
		Last Modified: Thu, 02 Dec 2021 04:06:49 GMT  
		Size: 4.2 MB (4161467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef01a32bbeafe701640335a32963992267219bd6a13f945952f4ce3212002f2`  
		Last Modified: Thu, 02 Dec 2021 04:07:26 GMT  
		Size: 48.0 MB (47984485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0172e0d4d1c1f19d4655aacbea408e67df8eb8475b1e7621eb9afb92ebd7a3df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102119996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432cd3c1456be6f1af7d50578878f66db074e4c02aa841ef6d3d85ce0aae9b1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 11:50:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbec5ebba783328c4a3d0185ed6fb278e4b0e213b45422bec84a45fb0a7b908f`  
		Last Modified: Thu, 02 Dec 2021 12:09:29 GMT  
		Size: 46.1 MB (46125846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b3b2fe296b8ad3041403f0c3bbef8010597fee8185c5a025ce541daedfb115f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105000018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acbc7bc0492da26e7e9f6bc28512bbac8acaedcdbec5dfd88b1b019bd7b7b96c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:17:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66df5c57061d26479de8f7ee3e37301f5bebfd97c94724dab3e21918f41f749`  
		Last Modified: Tue, 21 Dec 2021 02:26:32 GMT  
		Size: 47.7 MB (47735273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23d43a9c448386ff204c462352601ae3f5dcef063ceaa1eaa923a51b0435d8cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113286917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:151f1f45496f6a8e8d22f12d112ea1b2ecbb1efb58f1ae47c92fe4b8d8e50211`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:09 GMT
ADD file:55bfa1f20811d5ad7e0824cb8b85e2d7c75ed74ca2784dae41a80c54c2ee3ca8 in / 
# Tue, 21 Dec 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:19:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:19:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a33597723b77b33e69ce15c675459677dc40eb6b8b822c767d1d106fb2b0365e`  
		Last Modified: Tue, 21 Dec 2021 01:53:18 GMT  
		Size: 46.1 MB (46097707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c51fce1ac683ec95f0c86c7641f827f198b990803f717ccf546687b4be861`  
		Last Modified: Tue, 21 Dec 2021 02:30:36 GMT  
		Size: 11.4 MB (11359468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8196c269478417443ffdcc48080de94b4136a900f548611f282dc723b34ffa4b`  
		Last Modified: Tue, 21 Dec 2021 02:30:35 GMT  
		Size: 4.6 MB (4564918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0103767f9e30cdb022f48ed2587254717c334195519f35285c473ce97d331f7`  
		Last Modified: Tue, 21 Dec 2021 02:31:01 GMT  
		Size: 51.3 MB (51264824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
