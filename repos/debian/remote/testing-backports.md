## `debian:testing-backports`

```console
$ docker pull debian@sha256:7f3c702fad5106de8e420df6ef722fae2ceaffbc808268fc3ed80e9e1b67e959
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
$ docker pull debian@sha256:3a1ddcef1cc18d5a1d6e733b8a1850f12fe5e2ae549014af534a822d43f11cd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b6faf0763307f8ca520d0e4d5df4daf66757caf547a185f7a20789e248d95f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:43:13 GMT
ADD file:6907a2ebc2a0aad5206633c002bf737eca43ed9f0dd72f5211254aeee03153b8 in / 
# Thu, 14 May 2020 22:43:15 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:43:29 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:40308aaece740bc9d06b36a9513e7c4648663655241d7d0317b7814f93a92e18`  
		Last Modified: Thu, 14 May 2020 22:51:21 GMT  
		Size: 49.4 MB (49359485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5b95f4c80d5d5c27bfdeb5076a822b0e9b9f8b36cd99fa39f7154c51cfe856`  
		Last Modified: Thu, 14 May 2020 22:51:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:422875ae755132368186536c163776bbe282ae85ef8df12ee0fde751142f6815
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47161744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fae34d0bbcd5d28beb429c87c359832db7890c0b22fd8c1edc5f61996cd864c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:07:30 GMT
ADD file:da3cb2c22df2df04f6f47b2b21857b1c5193b582e3ba40ac3387c8b6fc5b263d in / 
# Fri, 15 May 2020 01:07:31 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:07:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6ab5f95a3016e564f5daec5899efa8267e4f47409ca71d02fd9044879d6ab399`  
		Last Modified: Fri, 15 May 2020 01:15:26 GMT  
		Size: 47.2 MB (47161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a993f007e8f697a7b9ddf7aa9422ec3e754b3a77c92d1a8bab9ac76c3e2ff5a9`  
		Last Modified: Fri, 15 May 2020 01:15:33 GMT  
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
$ docker pull debian@sha256:6563d6a9b48305cb0a89ac60d358c768fe909aa1fe4f8574abde5bda88fb74ba
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50132078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c156ddf94ff9f538e259007a3d6ea40f712024b75362dbd7b4425862f2c5c4ee`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:52:27 GMT
ADD file:4e6f3e92d41c6a0be8e697bc8e6c52cdde2c71a151efe2b38960a8350c91860c in / 
# Fri, 15 May 2020 04:52:28 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:52:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3d413ba2d94704c8957c0276cb71400c7c7d6f37305f7ccc6b13f171e7dc27d0`  
		Last Modified: Fri, 15 May 2020 05:03:21 GMT  
		Size: 50.1 MB (50131856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadebb0d18d5e9d7270596009ebee8d458058fb05683a054d492c4a0c953e3c5`  
		Last Modified: Fri, 15 May 2020 05:03:31 GMT  
		Size: 222.0 B  
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
$ docker pull debian@sha256:e0b1cdbbcec4bc9b4e8a13c9d0dab00420a1121da6772914b7e8d25543f7ffc3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50002814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5beaf71f0776192ed2eb42cfe9e5d67d69b14629958ffa35fde2bece9e3168`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:08:55 GMT
ADD file:e53c6c90673c558baee5d1bd63e6ca55daaca8afe6d5de578ca3ed71cfb77a6b in / 
# Thu, 14 May 2020 23:08:58 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:09:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9b48b5be91ad08b23c8cb04a0851ad6f8d9d8c166365a291e9766e147dd9c1ae`  
		Last Modified: Thu, 14 May 2020 23:13:16 GMT  
		Size: 50.0 MB (50002592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5347a385b62dcad85689620740cb0ce2ede8c09d44ad484b27b1be5b7e9b85`  
		Last Modified: Thu, 14 May 2020 23:13:21 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
