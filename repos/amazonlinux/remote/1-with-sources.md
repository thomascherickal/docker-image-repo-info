## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:f6dc1046eb8d41c757177414c99b795644dc61483066dd074bd487fd1ae6971f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db6f5b872cf347550fbc84997035060cb3f29b4092a502414aea35e1614a58d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515032600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de55c246e0ff336c46024f08fa4c8a76b99da444999c63a7a28e4590eafa6608`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 10 Feb 2023 18:19:33 GMT
ADD file:f748cf37d9bb118581db4644923fc7f81aeac9af93188e42a5c85bbbba9770f0 in / 
# Fri, 10 Feb 2023 18:19:34 GMT
CMD ["/bin/bash"]
# Fri, 10 Feb 2023 18:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2f3f7e5ea9b509a345d00531d4b8504f7720dde9cae889e01f4d4e8dbc71db34.tar.gz"     && echo "717d08c398cc28d075ab0ebe75c3785a5277a51c6ab89f5a959b7f1c7d2b98fa  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:42f354128e7b08a45107942fd4ecc2977b7144b5ec9a6c343c288a99da208911`  
		Last Modified: Fri, 10 Feb 2023 18:20:39 GMT  
		Size: 62.3 MB (62267134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c8a964734f86273bdbe5f0d0815e887a76e38d1cdcd222072559d44584cef7`  
		Last Modified: Fri, 10 Feb 2023 18:21:31 GMT  
		Size: 452.8 MB (452765466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
