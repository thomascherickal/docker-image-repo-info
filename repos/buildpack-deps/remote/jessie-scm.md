## `buildpack-deps:jessie-scm`

```console
$ docker pull buildpack-deps@sha256:41db0f68142d2478be2fa8da7fbc788f55274c494002a60e528b4a9e668ff762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03997f0b753d0e972b3d35390033eadcd105ba15a11d8879fd90feb02f420d84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115268710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f40cdcd7d07320115435e2c2ab0d0de4a665cfd420b5bc5bda417d1810d437b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:09 GMT
ADD file:0419e8fcec7ce7e70dc1f1e19558f15ebcd61d43a3b9955811783ac3a56c79ac in / 
# Tue, 09 Jun 2020 01:21:10 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:49:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:51:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0cd7281e66ed488ba431fd1e41a3c5fd628ed921f059ddbba2597487962ab380`  
		Last Modified: Tue, 09 Jun 2020 01:26:04 GMT  
		Size: 54.4 MB (54388052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041e5427efd77699a148fcef4a48824bba787ed6c2db375aa3f3d8b97ac92ad6`  
		Last Modified: Tue, 09 Jun 2020 02:00:55 GMT  
		Size: 17.5 MB (17545709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd1bce0fad2e8c8c996f62251321b38f07c985eec3022deb89a6d9d2d33932`  
		Last Modified: Tue, 09 Jun 2020 02:01:08 GMT  
		Size: 43.3 MB (43334949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6f0126ddbcb5315b6af254671036f76b0c34b960407fae027288b6ce5a203da3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110774844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324814b22db6d9a91d2919224a8b9a31383ad91bc6fe1a7ac126b8e97cb2e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:52:16 GMT
ADD file:4714dbb428f38b9b79a0b0234718dfa1c624973506e8a75c52a1753f4202bf13 in / 
# Tue, 09 Jun 2020 00:52:19 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:33:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:33:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:35:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d40938239771bc3bd6ddf7de365dee7a73a438f26b51bd64c09fa994cda5c2a4`  
		Last Modified: Tue, 09 Jun 2020 00:59:47 GMT  
		Size: 52.6 MB (52581526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5029f3fc63be5c726f83ec3d4ab5012e35c3267c5eaa1e83f1614de2fa36622b`  
		Last Modified: Tue, 09 Jun 2020 01:59:39 GMT  
		Size: 17.0 MB (17037281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440d38088bf0cd4439b7454b48c07c745841f10b8ae034fe13636553f0d6aa6f`  
		Last Modified: Tue, 09 Jun 2020 02:00:00 GMT  
		Size: 41.2 MB (41156037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:93538f441c10fcea50938f84d4ac8093b6ea69a4e1cb29af75c6ca0a09906d76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106806387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e706f5190a307ff0327fe6cf9757b2693c9ceba4197cf6be6e74359c9492a86c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:53 GMT
ADD file:e29fa406906c6574ad0eb78b933031cfcc111886562a056ec9634129c964dc87 in / 
# Tue, 09 Jun 2020 01:01:57 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:53:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:55:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:909e57799b0753688e459363ca5a8b3b97160ae637423d0533fd72503e5ef9a3`  
		Last Modified: Tue, 09 Jun 2020 01:10:48 GMT  
		Size: 50.3 MB (50304486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be3c793af972342b8657d56ce6f318a17f6707d23555d7407bde9347f0349ea`  
		Last Modified: Tue, 09 Jun 2020 02:12:44 GMT  
		Size: 16.7 MB (16723388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dadf04af03a5d22b88d6e1682515b77bd2de6c1ce68c80712fb63ce0df2065c`  
		Last Modified: Tue, 09 Jun 2020 02:13:05 GMT  
		Size: 39.8 MB (39778513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5387bd6921e9ed48d27a3662a617f469c35dca2d0c898ab330ccc7833dbb3cff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118453677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4a94efeba3656da25954d64d2414191a3096a22aa25da57154104ad8eb6910`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:40:03 GMT
ADD file:e6be478576ebd8d188f0f0507591d45863e225be60ae0e6381a7c54446efe116 in / 
# Tue, 09 Jun 2020 01:40:03 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:15:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:19:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f753419b4b3c0070d8de5c715f2097d69b60f7b505cc1c31085c9871d67952d5`  
		Last Modified: Tue, 09 Jun 2020 01:45:23 GMT  
		Size: 54.6 MB (54607842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c6dd78519f2dfee7b28710545708cb946bbad983c2e4327254a388e0e2b024`  
		Last Modified: Tue, 09 Jun 2020 02:33:35 GMT  
		Size: 19.9 MB (19855839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6d85ba7b1ab6cba5194944d26a4436d3039d76f3a26d0bbd94c3c787ee8e2e`  
		Last Modified: Tue, 09 Jun 2020 02:34:00 GMT  
		Size: 44.0 MB (43989996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
