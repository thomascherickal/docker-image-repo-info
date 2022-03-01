## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:ab839e170edd95341cbe8c52a6c6c002200f59b9dedc0b2fceaa18a0a134b8ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9b7cae82f76df063116f527e04503605dabb34d0fdf6b4ab4e3edd683c647dc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110788141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482d271fdeec3dc77e3c2253952ce97fb60df11dab97d6bb82afe13993f8b819`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:15:54 GMT
ADD file:23c8493cef4b2584f2526f870645f80d71b4572c29b49a264cea842d2aa2ee28 in / 
# Tue, 01 Mar 2022 02:15:54 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:31:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:31:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 06:32:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec52bb9d0b765b0726e476d07a8d9b2f808cf7b380f27c1544afa286fe5578cf`  
		Last Modified: Tue, 01 Mar 2022 02:22:47 GMT  
		Size: 45.4 MB (45381330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289049e62eb62ae7bd7a8f612cd5b42f36d423951256750f08baa96922b8587`  
		Last Modified: Tue, 01 Mar 2022 06:40:06 GMT  
		Size: 11.3 MB (11301983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e926c3d7ccab64c93f5552646ea61693989e06e27abf8cfdcbd0aad8e78c71d`  
		Last Modified: Tue, 01 Mar 2022 06:40:05 GMT  
		Size: 4.3 MB (4342352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd63791ebe323af1573a61d3e6c93bcf5c12da3b8603289c2b9e8825b045bd3a`  
		Last Modified: Tue, 01 Mar 2022 06:40:25 GMT  
		Size: 49.8 MB (49762476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:495c748fa9bb341cb1263c8dfe7fc122b5b3cd66ecfd151f5d24d660ec639d98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106593991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7814a260ed80a574677457a82b45a28fefcf3065113cf5551c1c30bc365715c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:13 GMT
ADD file:ec0901c267c269fc577d7b4fde4613c524c414738129f0c66a6e4f4939149fa2 in / 
# Tue, 01 Mar 2022 02:08:14 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:14:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:14:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:15:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c2dca75d28e97fb60ac629a75f7314e766bb9e4e8ae03915f095495736fab332`  
		Last Modified: Tue, 01 Mar 2022 02:25:36 GMT  
		Size: 44.1 MB (44091861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8d131bf2041d83b8f317c63f8e01f69a924b66ac0aa8ed768bd2f11e26d2c7`  
		Last Modified: Tue, 01 Mar 2022 03:33:57 GMT  
		Size: 10.4 MB (10352125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487098dedb48cbabcdd4ff9ead2ab63da4b7bc9a851f9c5e49d9795d693120ab`  
		Last Modified: Tue, 01 Mar 2022 03:33:53 GMT  
		Size: 4.2 MB (4161406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9af62b3e76cde8b5751dee3233b9326abf500680b5a0b22a5d0e86e39405c55`  
		Last Modified: Tue, 01 Mar 2022 03:34:44 GMT  
		Size: 48.0 MB (47988599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:24f7334efc5b988c07f70e311095ebfec07d13d4fbd8d239945b4f6098f1e9c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102120638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb23fc8a85219b2962eac54b9ff4ab53279af8b1bea3947198b186539efd5b65`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:34 GMT
ADD file:2d0ec7b989e0ef6e7c2d7cdfa1710507ce32d2218c0769aa5adc804e485973dd in / 
# Wed, 26 Jan 2022 01:47:35 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:49:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:50:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4becb4205b812ec841e47cdf4840f3cd4afedb320617c1a611bd7daacd1b1e2`  
		Last Modified: Wed, 26 Jan 2022 02:05:16 GMT  
		Size: 42.1 MB (42116772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19142ccd43f320261157cec769910c598094bd2f6235ca3fb72f11ff969ba877`  
		Last Modified: Wed, 26 Jan 2022 17:12:46 GMT  
		Size: 10.0 MB (9956581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc45f0a06bfebcf8cb3dd7f3b1577bb99c1c9a19b3dc44bab307cdd59267bb`  
		Last Modified: Wed, 26 Jan 2022 17:12:42 GMT  
		Size: 3.9 MB (3921220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f5aa09ea754ba47aefee810b542e69d5f77d134463813ea07489fa9ec46932`  
		Last Modified: Wed, 26 Jan 2022 17:13:26 GMT  
		Size: 46.1 MB (46126065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dea906b00f22ed3e5dfd17b8ad9270affd1b4da4141050a527dcffb9e9cd5508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104998486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b1c5ebb55c0bb566b9bf271293ccf1fd364a606e6c324a84a25cc32d05a8be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:34 GMT
ADD file:fc57ceb549dcf9223a7806f1dbd83ede31ad1705eda04387f43795b8949b19c4 in / 
# Wed, 26 Jan 2022 01:44:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:18:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11cbe372cf332799e1339b2b8a04723e8224eb56d69212a1308d1df0da55eae2`  
		Last Modified: Wed, 26 Jan 2022 01:52:53 GMT  
		Size: 43.2 MB (43173725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf576a0611a8862b3ac5cc25b79aedd7b2f5a1a457ead352a467fa5b906d0f6`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 10.2 MB (10216892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc21f7f695aceaf60c5d2590b7acb0d3937aab7af8a9470dd74605632805610`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 3.9 MB (3873916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16466baa01cbf2b86dbc5f9f876247c80462e423aa7a6b68dfec79de47f85e9e`  
		Last Modified: Wed, 26 Jan 2022 02:27:43 GMT  
		Size: 47.7 MB (47733953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7a354e84d4eea6efd587d90e90f5509c734d7465fd18160460e0dbdee1cc28c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113288140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dffb1b60e3e39c58791fe4c8aa2b802d3dc1cc9ba8933f2e00dd9d9c85f7bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:10:13 GMT
ADD file:bc15f0e456e3757963e61c9b01f81ce157b35fb751d837cf7b6ddd9277872821 in / 
# Tue, 01 Mar 2022 02:10:13 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:46:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:46:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 05:46:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d460050f4b628f05281226d933aa11a10afffc452771e0d9dd815bb6858e254`  
		Last Modified: Tue, 01 Mar 2022 02:20:11 GMT  
		Size: 46.1 MB (46097796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f57a4965e785e81bf52d7df87a7b3b5abeeb384075fef0b195b12bdf3864206`  
		Last Modified: Tue, 01 Mar 2022 05:56:48 GMT  
		Size: 11.4 MB (11359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc782b42f9af37d9d74bb076c8d6bb03945730f16d04982ff3a85814c557f12e`  
		Last Modified: Tue, 01 Mar 2022 05:56:47 GMT  
		Size: 4.6 MB (4564923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d56af1c75591c3524a488450e5adc45a5754e8c91dbfe711564884f78bbc6c`  
		Last Modified: Tue, 01 Mar 2022 05:57:12 GMT  
		Size: 51.3 MB (51265739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
