## `debian:testing-backports`

```console
$ docker pull debian@sha256:fb3a9f02a2ffa2d7dafcb30f888177ef54cdf0f6cdf0d64faa462c08658bed06
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
$ docker pull debian@sha256:cbfa262d0bb0deb3022c38dd88990ba6fd8a3365fa222cf296e29afa0dc4d94f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51384921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1529a50f0060c5269ee8cf3ff81db8c2f1d141609c5bbd9cce1c8be6af71505a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:24:10 GMT
ADD file:938d55a7f9952b6fc3027163d5f884022164852a3f59a887cd72fb4abd480b23 in / 
# Wed, 13 May 2020 21:24:11 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:24:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d99ec7dde2bb00323766bedbab11c8b41f0df40356503056ed3719e70353c12e`  
		Last Modified: Wed, 13 May 2020 21:31:05 GMT  
		Size: 51.4 MB (51384699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9590650e16391149bcba892a5a9a6b020b8e338e8aeb000d9e5e34b48fc5294f`  
		Last Modified: Wed, 13 May 2020 21:31:09 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:52fcb269de5cd1f06005ed3d78416f8eb12a0b9c38963195e5b2fbbcecfaf8ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49358670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fcfa53a30d9e02fb75696486a6421e7c6e58b21d18ffb45e0a2ca0764d3c8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:55:45 GMT
ADD file:cfdfdf8babc1dd6a29c1b28d04d021d6ab0c544eb73f9ce05ea155a0c605c087 in / 
# Wed, 13 May 2020 21:55:51 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:56:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:474643a30a55b4764ed792f4e1f68822d163caa16cb50fee8aa04da5d1d87b38`  
		Last Modified: Wed, 13 May 2020 22:03:49 GMT  
		Size: 49.4 MB (49358444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c0b0d3905cecccf7582c4ff14694b754a9bf901046f607c0fe5684a6b9fc7`  
		Last Modified: Wed, 13 May 2020 22:03:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:cd141e80311ddd549e5306e68b2c3b4a2256c3866dc348e1cb919af9c5281643
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47162495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9e64235320fc597edbd75637889577fe22de9834b6b31f76296a8799dab7f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:48 GMT
ADD file:a6656c1767c3aa4fa4364e9255bf59baecf3e1b14d11c5e62bed663be2b60315 in / 
# Wed, 13 May 2020 21:19:51 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:20:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f3745b1012d32d87e17173996f83b450f6566bac778d26d73bad946652d4408`  
		Last Modified: Wed, 13 May 2020 21:29:00 GMT  
		Size: 47.2 MB (47162271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142df78d5facdbf6b802e1daac4e27b5b7699b47a683a90bba681f93be3eb55a`  
		Last Modified: Wed, 13 May 2020 21:29:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:58d43bcb22f653b51d347349cf6833254a990b3ce80a4196bf2a6efcc58e2845
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50328550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560693efc43ed11a92d543eabc66efbc63a890b561eb3d6b362cef411804621f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:50 GMT
ADD file:fad35f66dbab8f1fa900228268afad338103bc98a5c9f92bc41bbc6bea004868 in / 
# Wed, 13 May 2020 21:48:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:49:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0445c2dc2fee2fa58135941f50318d855c2eebd7ce2e28ed459a7a498aae85b4`  
		Last Modified: Wed, 13 May 2020 21:56:47 GMT  
		Size: 50.3 MB (50328325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650158c9ed7a1de9dfa5f4459127f5765183016930c732ab2df880222f4e37a3`  
		Last Modified: Wed, 13 May 2020 21:56:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:6b8c638363dc50589150f65d99e82920e9936756b5187d87706e7eb8d8592aa0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52480502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26e3a4acc3dc0f5b4938000ebbaa175f797fc899f3bf88a7957718db64afd0ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:58 GMT
ADD file:1391d6bcefa66d06d38c6d12cd42e7b8b9a6c9828759b465d6d7ed1d7c4f286d in / 
# Wed, 13 May 2020 21:42:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:43:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ddce73e4c851a74eb19cb407063b2febe6d6c618c5a35001c4dcd11157cc283`  
		Last Modified: Wed, 13 May 2020 21:50:37 GMT  
		Size: 52.5 MB (52480280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c9d12fe635e6a732b61a99370f49f8e8287813c3154c97893285d1db36b072`  
		Last Modified: Wed, 13 May 2020 21:50:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:cb236a832d90e4cf60ae18800c24973ba646e1c683b45e4653c954beb54ff610
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50131356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20c7be1edd45d3103836d819f298ed329d03ccddd80c380e1173e701ce85a47`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:53:04 GMT
ADD file:475b54c279afc3294d39106302f257f5b08aa2e1a125452614da1cae38ea184f in / 
# Wed, 13 May 2020 22:53:05 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:53:12 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:042c6acedabf5b5bdaa9a3f858a939b8644165457a5bb35a34265f8059c9965b`  
		Last Modified: Wed, 13 May 2020 23:04:01 GMT  
		Size: 50.1 MB (50131132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2eff1ae3928ed59ffa23f7d0e1271d96d2e9c8474dd8b7e071c9f9ef506161`  
		Last Modified: Wed, 13 May 2020 23:04:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5fa444658dea7610d8d795e715fa40f45cb8b0c19244bf875549e41585998fe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55110504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fdbea3bf5dbd9064a55c4f8e1598206f5390fc4694e2306e09941274d6ee37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:45:20 GMT
ADD file:421f00a6539e893e338560c1d8942df0ea167994644388f4c0d5cc17fcf0e00b in / 
# Wed, 13 May 2020 22:45:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:45:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8ed549ed3b4c95d4c9a923179bc6fa471b69852d4d0483e0c8e5ca1cd7a9a622`  
		Last Modified: Wed, 13 May 2020 23:03:31 GMT  
		Size: 55.1 MB (55110278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0b4121ba7d21d6fac9b95180799c7e5655bdbb06d04bc55203f26d545c68b`  
		Last Modified: Wed, 13 May 2020 23:03:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:4c03f1510ef05585245cadf16e425142f64cf255118ffda28d50c56d5d1fda45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49994829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc4e3ec9f62c768f3f9cb42e1b55cc95477fbdd4523fa5b7a0c0a65a848b8cd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:44:50 GMT
ADD file:40041ed25d3ed86e018b850d0e45e1e094ba0affd730cbb11aea89a2387ac0b3 in / 
# Wed, 13 May 2020 21:44:52 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:44:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:71e274023239ef09a855049eb6057cca73c68b812ba6c77921eca009476d9d21`  
		Last Modified: Wed, 13 May 2020 21:48:56 GMT  
		Size: 50.0 MB (49994606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9613baac64eea63e98093d15af81ec73c6767fb265b2e2268fa7ccf87d1372da`  
		Last Modified: Wed, 13 May 2020 21:49:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
