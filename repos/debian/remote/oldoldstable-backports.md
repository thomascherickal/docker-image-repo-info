## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:6e14d71840652f41694eb496ede9637d4ea9d6c4e894c3c3e42b9a1cb5e9933c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:f02dcc759e2d85fdf5d019ea48bd28a5a27c6850695543039472564519d55798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50497797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cfe46424b49f342df41ffdf58d1d19e7d2403ee19c3c2ee372c5784ee55beb4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:44 GMT
ADD file:10ed85ed93772b28f677edd76ba09d343fb04cdbed334f43420df78e7e8ead4e in / 
# Thu, 07 Sep 2023 00:21:44 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:49 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7d56f470020063569238052abd3509d7102e670712674742085e41b308e04495`  
		Last Modified: Thu, 07 Sep 2023 00:27:02 GMT  
		Size: 50.5 MB (50497571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff462f732a8327f3627108bbeddedb40acd97b50d6508459e339ad8e72fddcf`  
		Last Modified: Thu, 07 Sep 2023 00:27:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:357f98bad35dcc177dbc02ec1fb1dc10cb38a4ae1f550bdafe57939176c11718
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7e79c3c035d1a828cff99483659645bc7c45d1177e6a13fe7175bbacc8c375`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:43 GMT
ADD file:75ee6f7a88f5ae0616421a89c73656a7d9a67bcf9bf488626e666a86d6632d24 in / 
# Thu, 07 Sep 2023 00:58:44 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:58:47 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0df19f4c8984022bf3df85eb20c32fcfadc42cb0d15bd0dce8cfc0abacefcbb5`  
		Last Modified: Thu, 07 Sep 2023 01:04:12 GMT  
		Size: 46.0 MB (45966105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8a0df992990ed6ca5309e3e2505c122b76ffc9fd4761a7909c1d5c8e81e23`  
		Last Modified: Thu, 07 Sep 2023 01:04:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:86c95bc2e233769138cb04ffa304fd63a431733ca2c56bce2c58e158b6737ca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e810868a61c94090fc25d8e2504171cdfbf714b4a673624ede3f48767d7bcd6c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:48 GMT
ADD file:c668c7566bad38acdb4cf94903133ade5ae2602eaa3bb92123e69173e4d3bffa in / 
# Wed, 20 Sep 2023 02:44:48 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:44:51 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:51fc984e0490aa8d77ad122fecef1f9ce0ff384dd3acca4001f69a1ac8068918`  
		Last Modified: Wed, 20 Sep 2023 02:49:06 GMT  
		Size: 49.3 MB (49290912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c514941c74706b5272c0b3530b0a1941299b6c6eb3e4a388e550d173890da24`  
		Last Modified: Wed, 20 Sep 2023 02:49:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:90b9400546ddc6e36fee14cbb119b8425bbdc0a379cc1cb217d7fd8f9a2e316c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51255670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e87a2b298b4489b95b2f5475da220585ae660fe08bc934584bc9ac58d7749f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:54 GMT
ADD file:b87f3f07a723e87d90b68c40c013ef63eb20e4cd00411cc2d451db9ebe11fbfd in / 
# Wed, 20 Sep 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:42:57 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e1039ad7b1b29f5886c8db391794e5be16e8cf8fa37f81c4c77009faf0a1521c`  
		Last Modified: Wed, 20 Sep 2023 00:48:45 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd300e8269debdf98b66c9baae97103eb7fc478cf7843bdf3ec28d9ac797e97`  
		Last Modified: Wed, 20 Sep 2023 00:48:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
