## `debian:testing-backports`

```console
$ docker pull debian@sha256:2d6cca417f5f883af30ad48122d905dad5b7447a2a4c4e3741fd3c5096d113e2
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:9832a0f35d5cfdb8fdbf88224cce9d89393e8f1d12a054d7c423a95740731b1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54898355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c60b8b8e75f3928b603f37023c66ec386e8c4cea68a25fd4c2c112b0c2d145`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:26 GMT
ADD file:11d79229fbf81be2e84ec81659988987938f28988fef7b98793d53f36f1210ae in / 
# Wed, 23 Jun 2021 00:22:27 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:22:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e767ccb423aefb5241f61d2fd04a45363ff299f39c6474bbbb5a95ef4daace9f`  
		Last Modified: Wed, 23 Jun 2021 00:28:54 GMT  
		Size: 54.9 MB (54898130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4a8361cbcf286da4ed566b3132b0e69f0c75989605069bb2af889e4a285e4e`  
		Last Modified: Wed, 23 Jun 2021 00:29:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:dc6499f2bc3b42ccfa30a11b58e8c5c0dd1c85b8a7a93b0fbe4c510a86a8ee8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52438529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69655f96fcae7f0b65e3dec0dd74d165176019f75827678d56ee29a7234e6d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:53:41 GMT
ADD file:99ead13a0047781439f1a600d271de98ef98228469c38ff53b100e63fe3fdfd5 in / 
# Tue, 22 Jun 2021 23:53:42 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:53:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3c9e3ce8ebca4f9e77336e87d22cfff842b39a01163bc956e4906151ceff4e75`  
		Last Modified: Wed, 23 Jun 2021 00:07:57 GMT  
		Size: 52.4 MB (52438304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034041f1a7d35100e345b639055433ccb9969fb8c8a3d7304a20a93c7f1e1d05`  
		Last Modified: Wed, 23 Jun 2021 00:08:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:02cb9992ff635fa5e51f5bcd335454f7da23b3460b95e555d40ba5ad041dc700
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50099376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54bc3aa9ab282e257f055c7a1cfa50c1f3fffbb90e49e4c85b37ab2f49abb354`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:24:00 GMT
ADD file:1fbebdb74df07b80be13ebdb48a4639c06a512f1ba9a05db288b71d592c1d5da in / 
# Wed, 23 Jun 2021 00:24:01 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:12 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aed124ed1f2302803c25af66de11f15c1d685d09ec3a8182a6b4da91031c8d31`  
		Last Modified: Wed, 23 Jun 2021 00:37:38 GMT  
		Size: 50.1 MB (50099152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f60b7b3a6c1035689a015c6e93c03da357ad21bfe86b89ce425c9f5d0b6a7`  
		Last Modified: Wed, 23 Jun 2021 00:37:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a3e1ba5805d934acf26b173fce28e1b0afe4c2c98ee0e6c29e637cc8467433b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53582127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c088641055b8612eb48b62f2e1f9104ca9a36207a3364836c5b9af6bec91a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:21 GMT
ADD file:8b33a86eaea1ccad9ad34b736951d7b1fc6ad3dfe7fb2a6b433c966b551ec8f8 in / 
# Tue, 22 Jun 2021 23:51:22 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:51:28 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ebccb1b0cca36e353580d8c119fa9002e5804d4069c1f1c0f2fd0e41fc820a79`  
		Last Modified: Tue, 22 Jun 2021 23:58:47 GMT  
		Size: 53.6 MB (53581906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6928f98fee5e09d94367ff9ed08f7ef9baa93c7ec556fb819d2b8b41fe933`  
		Last Modified: Tue, 22 Jun 2021 23:58:58 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:324074d8198c25bf0e5d80cc3070421b1cef4856419de319de9f601962f5d532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55914783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b27c8fd8670ed71599c662d786666047a0be195c160ae3e50ddc25f15a12bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:40 GMT
ADD file:c3c6c2bf4d7b39d1cdfc0b6b89ed2967a4671d4667fa3b4b60cbf47ed9cec4f7 in / 
# Tue, 22 Jun 2021 23:41:41 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:41:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f15bdbc5fc1218022ecf21ee04ea1becb4a574b422716a3b6ae7b05622aa0fe`  
		Last Modified: Tue, 22 Jun 2021 23:50:22 GMT  
		Size: 55.9 MB (55914560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54134b990acdcea9ee756b1febcce5a041c90c88e86e6fd3dc5ef31f22fd0ca3`  
		Last Modified: Tue, 22 Jun 2021 23:50:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:0ff64c03108a0362577a54af5af5747f51a65ec09e24647e7c29003364ab173e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53153179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce7573f4bff76ef6766405fcb7783070502bde54ef340a60adaca214ec3a205`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:11:28 GMT
ADD file:fe448a39b125b3c5f16f9e2c868ab5bf9c93285c1399619d3f0afb1a6e95adbd in / 
# Wed, 23 Jun 2021 00:11:29 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:11:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e5ca771ee6811634e018151ed97c18cd8c931ea90237b638cfa43dc9deccf0f3`  
		Last Modified: Wed, 23 Jun 2021 00:19:06 GMT  
		Size: 53.2 MB (53152954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b62eb9aef7c1ff7d04e6983e4458c890046e4127ae42bbbf141d8cab727132`  
		Last Modified: Wed, 23 Jun 2021 00:19:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:bf743a614b7a320416ef49c103ffc86a4cf284242578fd3c412863367131ace8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58811106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb9e2e42976baae97c9ac60b186c42b998116a0f7d0d09f129846b2a6e901e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:32:46 GMT
ADD file:28656f702990628f6d707772374ea01524be92a90a4933972d4d211cb573d675 in / 
# Wed, 23 Jun 2021 00:32:55 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:33:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e3a7c042d8a7a01b6075e7fecff62a88da28cdebf0fd80952fc3d6159d785b4`  
		Last Modified: Wed, 23 Jun 2021 00:38:58 GMT  
		Size: 58.8 MB (58810879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7f06493619f9d1f77c4556e8085cf995ef2fce1d87b513e2eb326b254c5064`  
		Last Modified: Wed, 23 Jun 2021 00:39:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:240b50e73227cf9570943ce62b927fb74d2701cd28dede529e65809891f47a8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53183402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae192de55ff549bb1bc96a7229a014c9038a250c3c59fdb8dcaa1147628f4dce`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:51:46 GMT
ADD file:facd85bf99201bf801c84cbad25dd5ea3044aa2a35468e8238d75094a32b5f00 in / 
# Fri, 09 Jul 2021 02:51:49 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 02:51:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57de50423b857ec03e5f5da3355e55ed7303841fa03258a82be273a6f2046de9`  
		Last Modified: Tue, 22 Jun 2021 23:46:48 GMT  
		Size: 53.2 MB (53183178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686cb69c2553d74e1bcacb58720a3c23cb426cd902582b04853bd658b6771521`  
		Last Modified: Fri, 09 Jul 2021 02:56:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
