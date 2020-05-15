## `debian:experimental-20200514`

```console
$ docker pull debian@sha256:ea9e2f01152f0268f68a0224991d6a89cda8b8c9285f63cb509f4e538212d32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; s390x

### `debian:experimental-20200514` - linux; arm variant v5

```console
$ docker pull debian@sha256:553160de9701152d62830a1eae94d051510ae9544928d71bc12bdf4be8b5b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79348a931e55bc68a47f79f7a554bf58b70d05e187aa5df5012d7704bffe1468`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:44:12 GMT
ADD file:86dde72a0ab87a01f23f0bc2339837559b947f3e626920eaad484dbb2c920097 in / 
# Thu, 14 May 2020 22:44:13 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:44:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:20f4bc02075b420ec27f08f233c21d9dcd74f712769151e4335502e9da73aafe`  
		Last Modified: Thu, 14 May 2020 22:52:03 GMT  
		Size: 49.4 MB (49372997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393ad04afc168826c552d8f126cbcb90d6cd2d1f5aeeebee1fea7ae0cffae0cf`  
		Last Modified: Thu, 14 May 2020 22:52:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200514` - linux; arm variant v7

```console
$ docker pull debian@sha256:539fb1a793e86f7a6184bb5d59587d0f18b17add045609b08997b43560b4ebaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47179359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f6423a1801de9f74880fba742eeffb4687c043d3090da6ddf13700b7a07bf8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:08:33 GMT
ADD file:ac494be0ca3977b2a3709423c3215d079ca60489990f617442bc1e2feaaef977 in / 
# Fri, 15 May 2020 01:08:36 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:09:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8c4b84cd07640896256963a5fca29a1de58f80b738614ff11c35863be81331cc`  
		Last Modified: Fri, 15 May 2020 01:16:07 GMT  
		Size: 47.2 MB (47179136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed5b033bbc8655fe6f43694b0024d9cc8288a05d60b841ac6d60cf4dc04da37`  
		Last Modified: Fri, 15 May 2020 01:16:26 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200514` - linux; s390x

```console
$ docker pull debian@sha256:81826624045efdae4f9a1ebfb34f8cf02b2844029aa63e6ad5393a9cd1674477
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50009218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b6377a7c0d1f020995ea700a961e99dddf5cad3194eaea11f026a6826a603f3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:09:28 GMT
ADD file:da245d4a644af8aa0de81134d0b9b79e7ca32a2e5a0da0f1400f9d49406ff756 in / 
# Thu, 14 May 2020 23:09:31 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:09:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:46cb5dbdb9422f82669828fe57d0feb67f9a7457725a4b624517b2aaf6a255ac`  
		Last Modified: Thu, 14 May 2020 23:13:41 GMT  
		Size: 50.0 MB (50008997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59318f7fe6a1db54282384c66be0d6cf6e1bd38d2bde4eac022e6b018d21b49`  
		Last Modified: Thu, 14 May 2020 23:13:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
