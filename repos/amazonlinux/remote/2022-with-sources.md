## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
