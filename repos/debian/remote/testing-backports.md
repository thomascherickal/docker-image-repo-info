## `debian:testing-backports`

```console
$ docker pull debian@sha256:96652abcbbccaad6737118c78801e0ce2f3c24c7e26e0a675b744d65f435ae03
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:e9b8e4a918c2d8eb10631f3f955b6e8c37cd285336a3a32158e3510b4586f2b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55560918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da818195935728971405189920870cc1d9b724ce9a355443450b2dd7bb5454a1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:08 GMT
ADD file:0801e9051ecaf8cd32ba061e9d8b06c000f3416eecdd1b685aecf44171d2198c in / 
# Wed, 26 Jan 2022 01:43:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:43:12 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:921f230b928f5947ac783609306a9da6b4f3c2fbc1347349ddf2815475c058e5`  
		Last Modified: Wed, 26 Jan 2022 01:51:33 GMT  
		Size: 55.6 MB (55560694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae3a0d0901e48826dcae26259f7b536761b4805d0ed48eb4a2321980de8e19b`  
		Last Modified: Wed, 26 Jan 2022 01:51:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:84069254d06efd789f5b9fabb1eef85eea466027026752ee47adec68d61548b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53020511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9621a26a8b100da644a66543bda25b6d564d65714ac8ce562f69a86f4671e218`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:06 GMT
ADD file:bc994ac7e0b6c6dff44c18970c79b334afe2a7d46f09983ccdd1d03bdbf15710 in / 
# Wed, 26 Jan 2022 01:48:07 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:48:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a7191fe7861ff59b18e343f93f2ce576b82da2e04cdc41f42a43e7cf7c6b5404`  
		Last Modified: Wed, 26 Jan 2022 02:06:55 GMT  
		Size: 53.0 MB (53020284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0432ad21fefa4c42ceec58b27726d2163f8fe6b569dab37ff5b02ba32aa908`  
		Last Modified: Wed, 26 Jan 2022 02:07:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:cb395c68a1f170aa2c7dfbb95bf33bcecaef62a28871a42175ae1acaa29116e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50663138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:747be660ff5af29eff69f18437e415c1653b75173be46bfe0209a9ab0d95511c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:39 GMT
ADD file:cd79965f7e00dcf53529436b3f5b5af2ec4c90e8e9c12a590f37d0ff75ab42dd in / 
# Wed, 26 Jan 2022 01:48:40 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:48:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9c7a07c323485b503bbe09c781f6eae41042da84b29eec843bfe1288b354e6ad`  
		Last Modified: Wed, 26 Jan 2022 02:06:42 GMT  
		Size: 50.7 MB (50662913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e744f963cd72b35b149b457940f27e1ca37b1b3c190f8b183d49a2677111777b`  
		Last Modified: Wed, 26 Jan 2022 02:06:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1a12d33bdb428b15dc1b4fe36eb1e2d51c58e191ccbbc27d95ce3ab0bb4c68a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54535457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba5b20e957f84a7b1c7f4da5476e1bb5f38f9ae1ff217719833b2419a7cb986`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:58 GMT
ADD file:e2a2e74c475403cf5762c9f71f745200db9a82ef550eab75ae5846166ed389f4 in / 
# Wed, 26 Jan 2022 01:44:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:45:05 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f4e7f3fd67ab16803b5ea5353b9b4a6d7bba8d2329182eb0b5733c1178fa6b62`  
		Last Modified: Wed, 26 Jan 2022 01:53:45 GMT  
		Size: 54.5 MB (54535233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d10d5a6a3339f0d279c93c00ba9fa1dc5ed16e9316efe366e77f937648c36`  
		Last Modified: Wed, 26 Jan 2022 01:53:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:7581481c40d2b7bfcce76fb0285e3e4ea00442fc58acc00b9b17eed2c3ae8852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56598204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34af7a3b393a0ac6ef3040562c9eddeaacf15132b2a8bfd999230804633843cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:26 GMT
ADD file:f3e4987b22ab588bb032637f7e16bf169cd3c1613cf58526c188a86f23107c88 in / 
# Wed, 26 Jan 2022 01:43:27 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:43:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5cf0f3f6324a6fc2d33bd0a4b1a888167efa8882789b29df059ae2d5d8ad8a3b`  
		Last Modified: Wed, 26 Jan 2022 01:54:56 GMT  
		Size: 56.6 MB (56597979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f8b7ad70b86119c1eede152d441585477eef48207b67c89f63043889148037`  
		Last Modified: Wed, 26 Jan 2022 01:55:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:b7738ae5546c6e3bef0c8a6e453cfe7e519b39fef2b83d9828047ade88f9cac1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54262217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5516ac8e94f073e86b9c107468cebaa55c107f507987522441660396153d286d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:41 GMT
ADD file:c1887a966b8d55323b2552420eb8c31e481f0d74d141c51b30d618c4744d1933 in / 
# Wed, 26 Jan 2022 01:46:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:46:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f930b41d0fa5188994bd7173c442204f40db98782943bccdc73def7b528d0f7d`  
		Last Modified: Wed, 26 Jan 2022 01:57:16 GMT  
		Size: 54.3 MB (54261991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd79fb832565f9dfd7680c30901549906328788c5b0aaf4db3ca23b8e3142537`  
		Last Modified: Wed, 26 Jan 2022 01:57:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:bcb8684406066b9da831105408a2725b522fccb9c261a29ffc8f5fe265ead485
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59942517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04b9d06869548503ea376913c23bc085d8762ec1f0388faa08f03b00395e23bc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:50:20 GMT
ADD file:38c73ba90be6f58e3639e5d4ebbb9b3f61fb845729ac0dca30389f1f8d2c32e2 in / 
# Wed, 26 Jan 2022 01:50:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:50:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:abb89d61badc571bdc7c4a161a7fc8463ac6b8eb973d6aeff716f76edb833ccf`  
		Last Modified: Wed, 26 Jan 2022 02:04:40 GMT  
		Size: 59.9 MB (59942294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99789eb1598ddca5b77323bade3a2d380998a07767230c2d108d8a67ce41fe0b`  
		Last Modified: Wed, 26 Jan 2022 02:04:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:86b860de585715037e383f8c6d65e1a68ed127d82e5df07183e1c735d23dd902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53837424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5702d9a5fe8a849e7e737931c7468274902eaf07ac4bd848c71315a6cfbd9df2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:13 GMT
ADD file:ec893d9debde17497a94115ab0f6e0aa1d63b99e4dab72c79dad068001ab3194 in / 
# Wed, 26 Jan 2022 01:43:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:43:21 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3bd38112da17d75c9bf6693e6e4ff711f53159532fa2ffe2ed12029df107c34e`  
		Last Modified: Wed, 26 Jan 2022 01:49:35 GMT  
		Size: 53.8 MB (53837200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349258f9fac6c1be999b5302ca69843a58bc4f56ce0ac320730c13713d04e1ce`  
		Last Modified: Wed, 26 Jan 2022 01:49:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
