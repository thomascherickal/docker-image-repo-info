## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:0d867d7fc1501ce835923660262c0e91e6dadda605ab2441629afa0be1b4ad08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
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
$ docker pull debian@sha256:1b8967e6fe722c90431c45ddaf3e26b39b1b76b195f0b5ba5ea35619612bd467
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50440648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec583946279ce555a679d4cb60ad38197531d9ef4c4cec8c9844cc5bdd601b0c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:12 GMT
ADD file:6c6dd727b4a86330f0a001d48ee1e61c9cf1cccdedab9943b04dcb76d6cf737a in / 
# Sat, 28 May 2022 01:21:13 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:21:16 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dd8dbe98482f3149a0de07fe52d533c0231718f894c974fdb1a19247dbe58145`  
		Last Modified: Sat, 28 May 2022 01:26:59 GMT  
		Size: 50.4 MB (50440424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c27d4983be7da6352dc5557e70749ee5f3c3e6932780ed6ff17bfadb92a74b`  
		Last Modified: Sat, 28 May 2022 01:27:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:315a6620251c0d8971415ca776844472a2c76c48094ad85ec36af949d331c2de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48157746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69a491c68c6586cb44460c16bd98e93d2e80f3a73fcc05382f478179a370c274`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:52:55 GMT
ADD file:52714e05eac3ec4a580498eece5bc04180a97c91db34b5f384ad4269e59ca287 in / 
# Wed, 11 May 2022 00:52:56 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:53:08 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d34300cf0b997d5df249ea70a7fa8dedc9c567168af6538af7d2bf1f6a0e2f4a`  
		Last Modified: Wed, 11 May 2022 01:09:20 GMT  
		Size: 48.2 MB (48157519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bf94ce32e17fc2fd6d028ad76b949258e94932a25ca2eab0e18aa18d4e1228`  
		Last Modified: Wed, 11 May 2022 01:09:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:626f6e7fc4133fcf9df7862f89e64bc84993c4f227b80c03929c3a37b86517c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3fab821cdb9d70432b8257e1c8d5d535cbe6fa1c062de0390767436a317b6e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:02:23 GMT
ADD file:93e45631d7edd7e30839cc3137e870dfdc4bc0fc5a060e953578681692b58d9b in / 
# Sat, 28 May 2022 01:02:24 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:02:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:46186334d02ab25c1cf8d13de854c4896919f55590bd823ebfe91bb84ceaae12`  
		Last Modified: Sat, 28 May 2022 01:18:47 GMT  
		Size: 45.9 MB (45915603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51581bdf5dcacb1415375252ede1da967c43eed3b804ff08156b0ef013888c0e`  
		Last Modified: Sat, 28 May 2022 01:18:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:304123c9068078b07f8336d1fd737aff2755441d2199956a44ec062fefd2b5bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df8b745e46615134b1293feda6c50b33c284834775451b7ce9a0e0b4227ebe3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:39 GMT
ADD file:80d27c6c157fd32ac9b69d8d7115259ba021ed0d7447c50aec7251a3899b4b9f in / 
# Sat, 28 May 2022 00:41:40 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:41:46 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:08bc7b3927bd8e671ea9952e215bb10105ddea98cf2b83651a3cf922566aaee0`  
		Last Modified: Sat, 28 May 2022 00:49:28 GMT  
		Size: 49.2 MB (49229037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a049f923c4fd9744c9915898a0ad7eb06d9521d521629115c654090e316c231`  
		Last Modified: Sat, 28 May 2022 00:49:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:9ba251d25455c11c00d554a7b4ae4518b58ee133097199c62ad85a25ac2384e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51204449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b66af000d0e5c27ff1e0fd1c87c01de3e88cd593cd3c11de19c187d8242ad6e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:37 GMT
ADD file:1db3a01981cc79d71fa5a24eba6c14a72990ecc081ed01b6d41e493b63e95ebe in / 
# Sat, 28 May 2022 00:40:38 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:40:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5559dbed49d2bf17fd15cac89e8b285b3d786020b52e88da8688c6b99f993d24`  
		Last Modified: Sat, 28 May 2022 00:48:36 GMT  
		Size: 51.2 MB (51204223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f214f4e5e3c12689fe4c306a8e4323a8323d78242950c734f5633546831758dc`  
		Last Modified: Sat, 28 May 2022 00:48:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:4cd7b9e8559eb855d50de480d01a5a55a340cda9e7f61fc300fc27cc759564d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49073591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4c614653b050569beec574f515aa0ffb39a98bf3f8ca6d84099cc46292583f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:12:54 GMT
ADD file:eb19dea96494052de4c2ea2ee51deb090eb008a2a39eaa9e1a623f1e7626e3ed in / 
# Sat, 28 May 2022 01:12:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:13:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d31bc4793744d8e909ed41c309a0633dea29816d12adde39b5f4b34fcafd2334`  
		Last Modified: Sat, 28 May 2022 01:23:40 GMT  
		Size: 49.1 MB (49073364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799d8ea474d0531b52435746317c28a54835bd3466eb05bdf0840d4dcc2e0584`  
		Last Modified: Sat, 28 May 2022 01:23:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:f9b8defec7095603f88becd4a390a97a4f17b29a82b595fe7a9e0f6e4b2851cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54177244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27df5f3699a73c3703c831b2e2c3835dbc65a3e143e56ff0157951eea22c7dc5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:24:21 GMT
ADD file:f0f6279b8fd985287b5f3df9480f1840f5d0b4a3dc72e3f373b89757ef9a9077 in / 
# Sat, 28 May 2022 01:24:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:24:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a049936bd2803fc7c63adc8dfe2c2a7792bb32515dc427cf69787f3b0d352df`  
		Last Modified: Sat, 28 May 2022 01:33:59 GMT  
		Size: 54.2 MB (54177017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01444c9d05003105f5d9bccbf299bcf82a819ef0ef8f7fe3d31ed72d3b6b982f`  
		Last Modified: Sat, 28 May 2022 01:34:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:6be4457287dc2975ab5809d5bb1fd67411dc2b632474fcd510f1c471439684ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49007014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f5a713c73f7dcf337bffb30a2c53cb8dc8561defbeb66ef794750568bdf1c6a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:44:00 GMT
ADD file:bd5cfd4dc8d90cc91b330c8c19624771c01f1ad03a3a3ab3cd71cfb76d2dd66c in / 
# Sat, 28 May 2022 00:44:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:44:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97c6438ef1df635b92390f341cba00358af65b7c27e2bd11a4ef6fff81d5a77c`  
		Last Modified: Sat, 28 May 2022 00:50:36 GMT  
		Size: 49.0 MB (49006790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e018bf5713abbf9d45181c0fc3d8ae96bd8af4f9ca470229efa053079e601877`  
		Last Modified: Sat, 28 May 2022 00:50:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
