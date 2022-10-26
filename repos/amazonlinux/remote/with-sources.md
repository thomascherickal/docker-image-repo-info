## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:d8317c7ade584beb412079366b679f659198063efa81c3ba17d9b8217b35a10a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:18d4254908fe549a3b74fe48afee88802d42765cc8cdad730a1d31f869d6065d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486382082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1372932df6c9127867ac9e8a7db0a8f25d0e776f7da5a33592582813cce66cdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 00:20:21 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae837e2df6db6c81612d2da73f641c413ed66985e004a9a6565edcdb2b757a12`  
		Last Modified: Fri, 21 Oct 2022 00:21:31 GMT  
		Size: 424.1 MB (424075440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:666035ad6bcdcb3acd33d5a1149aa9f33326ba6a3d37cefdd07aa795400d2e38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724f4723c160d54b79d767819020361b49089bc3383b30d244c7a5e28b8e50ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c2dbbe36f82b868eeba9da518a5cd14946071330d0876e061dfde90df696`  
		Last Modified: Wed, 26 Oct 2022 15:28:41 GMT  
		Size: 424.1 MB (424075437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
