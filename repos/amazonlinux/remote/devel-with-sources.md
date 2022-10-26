## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:1b6a3cf78359d45cff778c0b542bf66ec0c9fc3c1735d0d3a4f60ae0d8a54911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:eb03889b4ba3cedac439ce0d5c9f27234109f71356684cf4ceccb8d9b245b5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387784962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20868dc236eb38a2f45fab9b54c56ea5f685204f68019e30fa40d04ec7381912`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 06:50:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86aea60721dcdf4beeecb63a8df31330acdac43fe37466a09f951e571d1cee`  
		Last Modified: Wed, 26 Oct 2022 06:51:50 GMT  
		Size: 330.1 MB (330130887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:add79a7ef50521092c54edb7de96453991711647a6c92bde0878cc5636c1b872
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386634148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92662e39e0c8fda60f06351346cb7d9246b3202be7f9f14ed4797d80dbb76e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c84b504a5a9eb81ea0f91ff34bc0580d5b054ef32fee37e1c6d39b19f66c50`  
		Last Modified: Wed, 26 Oct 2022 15:29:22 GMT  
		Size: 330.1 MB (330130885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
