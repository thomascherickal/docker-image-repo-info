## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:c67c6b6f547317882f1446c96a2834ece602c4448e5f726f95456b8e43e7e684
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:3ba6a6adf9684811c82762d6f13abeca57ca8231412cd26459528c8aebda57cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45376138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:654de8662eea41141473c97cb7e8f8c4ee8ffd4a7b6c6400b9be3ee4872962b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:21:54 GMT
ADD file:3f033759ecf4f9f8ddee21886062b624f8511b7a99e01ed461a9b58acea300e8 in / 
# Wed, 13 May 2020 21:21:55 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:22:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:59b366d43ab3533d278be192eb3ac246e817e5c4b252bc96b006f70489002af3`  
		Last Modified: Wed, 13 May 2020 21:28:08 GMT  
		Size: 45.4 MB (45375915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b8c15b517ce7c49e187658d4e2d5a5a058fc83a4840ec2f96489d04a81a3f0`  
		Last Modified: Wed, 13 May 2020 21:28:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f89f6d5f3746d1a8a07d23955fc14063c8cd1f52997a48bb5525df2395a6d63e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44068003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a28763bc5c401967b07f7035aea0dbe93e2fd55d2838ed3c0aa95e3d97e80075`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:52:28 GMT
ADD file:9aee42a13d893728b0f4cbd87b07ac4dcb879933452116a79f907bfd4447b1ae in / 
# Wed, 13 May 2020 21:52:31 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:52:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a281bf628594ac2ad9d97092536ae79a6337b69fb902125cfef99d375144e8c`  
		Last Modified: Wed, 13 May 2020 22:01:04 GMT  
		Size: 44.1 MB (44067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6712020b5e4f31010e62bd0a92a24d095b796919623874075d74bbf4b89924`  
		Last Modified: Wed, 13 May 2020 22:01:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:69b0cedb429659d1171c5dd88038dc5ca1f03a0c4be75be8a0c008fa84d02e25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42101318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9fafb7103e4b1f03f9e62ee95edba7cc6ff33363cad35def9039eb56058fff`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:16:14 GMT
ADD file:526767b325590a0f8a02381e60888a56aff5898096ae65f9a2e3e006f745f3bc in / 
# Wed, 13 May 2020 21:16:17 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:16:26 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aaa6b57fb1abea026233ff64408552563b7318cee7456bc83e642a390fb7ab0c`  
		Last Modified: Wed, 13 May 2020 21:26:26 GMT  
		Size: 42.1 MB (42101090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feca4f7eb1a7ab535b87d6bd01d1fef473c8bb7137ce209311013136e38636f`  
		Last Modified: Wed, 13 May 2020 21:26:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c8a3ec8d593bc76d3d32fe26c861151ba55306f323d772752df18603e8d23b24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43159178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a2229551dbc8eaf910064355df75e94274c78c627c511905313a8d8008e7237`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:44:18 GMT
ADD file:dec7fc852e537016129a47b5cc0eb374c6b09fd17076b51eb1f3d92cdd9ad4d4 in / 
# Wed, 13 May 2020 21:44:22 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:44:30 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:451c2749d61ce76b7d1709f64624274d850bfb86aea7dc0c21833feee377fad1`  
		Last Modified: Wed, 13 May 2020 21:54:05 GMT  
		Size: 43.2 MB (43158952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8b2672f85cad68449279f42973fe3652834731c736a6ef48f800f10431e4b5`  
		Last Modified: Wed, 13 May 2020 21:54:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:d32f013d4e820b31d3df84fbc2034e68f553ca25f3ad78eec324f6a8507969b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46095303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67edc4ce68baddc6e9c8f8208d016334d1fb110138c9d976d52cc5728281daeb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:40:44 GMT
ADD file:0d8e1bda846dbe61891a8d38fea02b7d3304008130f0132818eb558b722a5228 in / 
# Wed, 13 May 2020 21:40:45 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:40:50 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:64f43be8f622b6cd9d132f78bfe57a01056a97ccb47e0229ee95f598ab600c1d`  
		Last Modified: Wed, 13 May 2020 21:48:06 GMT  
		Size: 46.1 MB (46095078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1fbf3f65249ada8af4f73fc9815eb2221be4b1284d9110be4ddc594db84de9`  
		Last Modified: Wed, 13 May 2020 21:48:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:a56ba1c4b10ba6aff2b63f4110986850761ace524737b5b32f5dc0fc4382b941
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45049068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee411226509c4ddf8cfded598b0b43cc4cbb33652892e997ba926321cf2b4697`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:49:22 GMT
ADD file:e65d914af0371fbf33574a83972727a41909980b8d5b115870c29fa6b01df457 in / 
# Wed, 13 May 2020 22:49:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:49:32 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2536b37517c72da0fe97ea82b5e753beb16b87941b2f7d3071e7ae1ad6039fab`  
		Last Modified: Wed, 13 May 2020 22:58:34 GMT  
		Size: 45.0 MB (45048842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e1540be313127aabbeea5923510f82db770155201c206865c28d66829dc2e0`  
		Last Modified: Wed, 13 May 2020 22:58:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:74c9ad3400ad1107cb4d2b520fef0d5a657b8bb6a510bb5c356409f21a31319a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45646476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31cecff44695f5f3e47bbaecfa217f65fd6b01967a8f819e80ce8d5ca68a43da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:24:15 GMT
ADD file:6443a668a74fcf32c5f82767f4c12add1107287df828576bf5d06f38f8f75f44 in / 
# Wed, 13 May 2020 22:24:19 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:923a4cedc3d159656a04021e9503d6cecd76cc101ab226fda7e4a2ac888a1026`  
		Last Modified: Wed, 13 May 2020 22:58:39 GMT  
		Size: 45.6 MB (45646248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5485ef1e0a6864d57a87b0dd3731bac16ec4b4590d057483e812388365a56e9`  
		Last Modified: Wed, 13 May 2020 22:58:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:c51148d44a3437e2a7964362ea79f800d0e03d8233a5d692c1aa1618ee97917d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45232953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552c75415e5aadd66d8ebcffae37757152eabae10fa9b4d39ab4ec9b95bee7e6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:52 GMT
ADD file:6eada3f6291c8b2843feef6bd7934e5cc0a4617f452dda9417b98021c6570cc3 in / 
# Wed, 13 May 2020 21:42:54 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8445e75ca26fb9a771e0d8317d0d661b4224584c78f173a9dc1bb5b764e6f8fc`  
		Last Modified: Wed, 13 May 2020 21:47:13 GMT  
		Size: 45.2 MB (45232729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724964cfef1ff403093309ac2839b50c86b2a2f555def160acc893c4a711ba43`  
		Last Modified: Wed, 13 May 2020 21:47:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
