## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:dc78153d3ac0ba50c33d06615bde4ad459ea793c20ef2d95332a083895247523
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
$ docker pull buildpack-deps@sha256:4508b936776af3db3d5665252a1a1dc406d424b169c93138fc73309e0fbcea42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110785612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbd17451a038d2673acfd7c408326f811a61eca03e7f71130b56d47ffa1c53c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:49:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01c447bcebcc60440b9d84f429ded8ce8d836952f1061c96cce5047230ab696`  
		Last Modified: Tue, 12 Oct 2021 15:57:31 GMT  
		Size: 49.8 MB (49762475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3b6dcef1865cc1d9df51cfcede2b22a42810d59e1ed7f2dd6f1a2afdab2da382
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106589552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1b47c4fc7cd09da1eadb373e1b3639dd3ea6f0d0a7f277a6f9a3a1badf1916`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7dba6a3a04082e323f475e5868064ca168ce598cd050957112293ff0fd959a39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102122625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a3d6567755cb1502e9dff34cb87fcdf9f48f415f7df777575dd8ead758ec37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 18:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38df34fca09f092dbbe9b57c3c215fd84572924c049269f617cdc79e0e8be50c`  
		Last Modified: Tue, 12 Oct 2021 19:07:34 GMT  
		Size: 46.1 MB (46126075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9c1e7cd43e43670fe1f350da75e1fb17d84ee12262a0ca4a50e28bc4e69d033e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105229149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35055b08b062ab3a45ae326dd3105f396e28445072acb2b43a382c2296bdd397`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:14:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449e92d9f0601eac3dbf717abf9680c96962909ab07b8ccdb946cd89230178`  
		Last Modified: Tue, 12 Oct 2021 02:23:13 GMT  
		Size: 47.7 MB (47737903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3dd7dfec75397dae002735d04557b86aaaf641dbf609cd11f267f7740392d841
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113285816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10424f2f9fa56c237f5a1cb67f32e5286a03841b408bf07e8c6d4f87b5757030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
