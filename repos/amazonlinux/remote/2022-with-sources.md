## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:b8b8b90128962363b90a5b7ddd524b8151178ba15f3e5cfba15fa51209fd11ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:12ecc5ecdbe5395b1515094ad80bdaa720034caefb3d09f69c49ad7f28babcb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.0 MB (392016191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53819a0095a6146d5cbcd2ea2874c210e83cd0ef869a9539c08f245089f75a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290d90a538e5f8c06ed51ada1dcf0fa26fe3322bf1917b55769086b8ec613a0`  
		Last Modified: Thu, 02 Feb 2023 20:21:02 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:96adc3194bef5ff646a57b27439727c4f53a334f47cf2973687043efca10f972
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.9 MB (388864428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad9e3b1f44835b8b6c4012d13f132673ccf6e1411f4dc7af71a4aafd94dae17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Dec 2022 00:41:37 GMT
ADD file:ff147b37fd20344db08d3808c57eecb4baf220c236bdadf01d19a61f2dd6327e in / 
# Fri, 16 Dec 2022 00:41:38 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 00:41:54 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-0e18855df9605c619bfdddcf96efa95943650dc6711ca144db81c72f8588b1e5.tar.gz"     && echo "4c1c20829b8261183075d44fbab402138760feda6163ff22701792d88cd7649c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f3bff8cbe57b20ad8a63095a2b0c5d31afccc39fd7fbaab9b0c483430b38429a`  
		Last Modified: Tue, 13 Dec 2022 16:26:02 GMT  
		Size: 56.7 MB (56712057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4171f41219f5fef2d776d5bb54af7cce1b43e645c3df8c0a0edfba5575187b8`  
		Last Modified: Fri, 16 Dec 2022 00:43:26 GMT  
		Size: 332.2 MB (332152371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
