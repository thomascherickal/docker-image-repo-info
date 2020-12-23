## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:60eaad1a680f611c9cf9fd4f2a1ddad0c299a28a7688ca2875c2631036b1ff7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ec8b116cbc8e5f39d32cc46ab9d1823d413862a07e85ddb4dc3b9ac054bb98c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542851989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba507121a17fcae383da7f3fc6481ee5707835c3e67b7fd68edc64698d31b44b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:20:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130bba24cdc0c903b6d6eb23f3cb5fcc362f36af331045a285d5ccb0c74bc45`  
		Last Modified: Wed, 23 Dec 2020 20:22:24 GMT  
		Size: 480.8 MB (480844561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9c7588150eff1d7928416c7fafd35edaa4f1d03d663f0c7fdac8ac62de67c8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.6 MB (544552541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d28578129bba32d0a61dcb4c5ce73ca3365c60abcae712f3c4d2edd3009ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 19:40:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431b17c8d2c281dfa9b3b9f9880a6159a978452bed73137b8af89f04586250c`  
		Last Modified: Wed, 23 Dec 2020 19:41:41 GMT  
		Size: 480.8 MB (480844627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
