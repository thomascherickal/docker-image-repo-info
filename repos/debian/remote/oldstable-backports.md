## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:7a87f87e261afbf912c749b6a9db6f8d7db10a0f9fd3da531d053ab7f1b5f1a4
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
$ docker pull debian@sha256:6811c499e19a6fb9360a10df22064e55bff174c6e9d5c37aaac228689cc6260e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44072065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e733af377333cba2bc48f18d0c8a2d71410b25490f79ebf69d4a8ba9b9fd7b9e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:39:52 GMT
ADD file:6a3873172bb05469b39267e97faaa5a88b26d10163455ce92858ab00b41403d6 in / 
# Thu, 14 May 2020 22:39:58 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:40:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a02dc173a7c3af68f27ba7bd2c84ad3bd4f5bea223b3221684760db06547d99f`  
		Last Modified: Thu, 14 May 2020 22:48:42 GMT  
		Size: 44.1 MB (44071839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0173ca5a4fe85d95bc7c8740e5ff479329cc1d55cdebc25305d0520841d4ea8a`  
		Last Modified: Thu, 14 May 2020 22:48:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:02c5ba8b80d3c4eebc9b47aab2ea222ee2c58f54058aa8de5c4cfe3f9647d81a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42104566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82ba2063a6a6eac9af6e9191540b40649ae7316a3c8c83b334ddf44b9527da9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:03:00 GMT
ADD file:b70996930efc92ef82442e29285863d25b4752968a27e17713d02a049ae3a80e in / 
# Fri, 15 May 2020 01:03:04 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:03:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:968153165585368b1b1ab25931c78d0f5b0307ef01cdeeecdf94a2b9955c4c7a`  
		Last Modified: Fri, 15 May 2020 01:12:58 GMT  
		Size: 42.1 MB (42104340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f15308b1e219d0328fbdb103745bcbb6d999cedb03b91d1181b7e01b503b8a9`  
		Last Modified: Fri, 15 May 2020 01:13:05 GMT  
		Size: 226.0 B  
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
$ docker pull debian@sha256:8efb1077ad028523cc75acef0d3935cbb268f7634fc480e7fe4257e8ad324cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45232363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c245b53ff53e485f2a0159d01636c15c4d8b2f026d8960a17efeb32de3ca37b3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:06:53 GMT
ADD file:7bb64228e15ddc34d5624c8a3329ef68be997e4d299b95cceace485e00a24d8e in / 
# Thu, 14 May 2020 23:06:56 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:07:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b28e354f80f29bc9dbe7da5033d0a531dd9687922cabd20419a093a8bceff95a`  
		Last Modified: Thu, 14 May 2020 23:11:38 GMT  
		Size: 45.2 MB (45232139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27d67238a4eabfc82e170009c93727210a4f5c11ff520d670e04128e2b2ac3a`  
		Last Modified: Thu, 14 May 2020 23:11:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
