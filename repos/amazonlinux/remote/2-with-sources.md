## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:e65e726f83310347d83d7ffab3375e29bba9b4d2e3316dc22bf9f70776d4b4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:6a8ca270cc7529a3da4123ea10c0ee61bfd59b0e4a0db0928d05d4a45470b51b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542821098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc5900d56f8f33395ceaaba7e68666dae13a14d1a516ee4c6a1b084b4060662`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:59:38 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38882999dcccafe0e4f06565dae85913942fcb9b250a3858b64618e1ef7264a1`  
		Last Modified: Tue, 30 Mar 2021 22:01:05 GMT  
		Size: 480.9 MB (480874513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:86e35f42983fda1d7e6e62e6c9073f684a444c516f66fcecbc6d60ff261ef17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544534564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a0528e0069c1ed55daa082c5603b43018e3dce5c1286aa57cd143804c753f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 22:00:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2bae5111d32ce9495afda9ddcd94ec2757b716e7f208b5b45ea710dc754d3ec7.tar.gz"  && echo "10bf5fa5b0b0b808615283d2de7209c58c1521c81a4953383fea0c38e1b93998  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9e8ca57ca152eedd246bdea5ab367dbe81d57c888320293b11d62a4aff4116`  
		Last Modified: Tue, 30 Mar 2021 22:02:12 GMT  
		Size: 480.9 MB (480874526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
