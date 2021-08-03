## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:10a89e26c570e6e9673182484c5509396099ab492edd8cadef2c7e1f072df2b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6beffd46592ecbdb9e7bb63998a8adbe73203b2a0b6411cf1546046d7188b7a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542940673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867fa952e4d51ef0c41cf888e945cf0903a76806f0cd2ef2e9cff60d01357584`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:20:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4581db6484e98433b91089f32a94db775460fb253ce6e3204dfc7b3349e97a10`  
		Last Modified: Mon, 02 Aug 2021 23:21:38 GMT  
		Size: 481.0 MB (480974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:192eeb0e12a69e30106d70e84fb0f0d3486a79de43e92a9f24be379cedfd7fa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544521863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858173ea3067285d35fb6e39c53242ea58d9b08897493eada5f2c603ad966a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Mon, 02 Aug 2021 23:39:50 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e832e506d930c525d101385e90322663126ac63fdca0b7d3797be8c2f6efb8bd.tar.gz"  && echo "fe52788ded649399eb7ba6e867c4373d3eafc99b9353955de47a39408b8ad366  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cadb9bf01fac34b09b53130aea8878867dd024801d8042a65d7cee698eb48e8`  
		Last Modified: Mon, 02 Aug 2021 23:41:03 GMT  
		Size: 481.0 MB (480975009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
