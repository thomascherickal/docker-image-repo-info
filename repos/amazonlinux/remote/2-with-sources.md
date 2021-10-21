## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:9c60d0b0ed9c145c13877b5394d24504e120dbabd39a8e8be9f6806eb28174b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:166a07247bb683593f03a556aa010d3bc7273439f038eccee9b5cc0c48af3e17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.0 MB (543000923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f894820418645903e9eaf82e16f79a3234546d6984b9778f7a495e4373787ef0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:20:55 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9e2410667f949f30b61e785e22df92d79408ac9eca07635984070dda5b1f62b5.tar.gz"  && echo "38104879f82d48a1d2a52ceb37ad6275a2b26ab7596440d3ace779cc54d440fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310d2444e47af71010180a773ce686cc6dd57bc3285799bd0d06dbc6d567f827`  
		Last Modified: Fri, 01 Oct 2021 21:22:42 GMT  
		Size: 481.0 MB (481048285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:3eea61a0e363060aaf6efcc205010405838c6c927ac7335d9e7b719b52396dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.7 MB (544666863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7872fae8888e29da6789210a29c489ca95731ea6c681047c511583c9b815f6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 21:40:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e9fd3b1031f9a7540f8249e5d30e6439633e1eb09f394919e35ac5017ec18c93.tar.gz"  && echo "08179d9c712a9a7f501377be8ec5e1f7c229343a5bec655c93db62c623831c7c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0e87113240ad7af60957d04bccc7fd72a3ba5616639f468473384eb2c7c691`  
		Last Modified: Thu, 21 Oct 2021 21:41:29 GMT  
		Size: 481.1 MB (481059985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
