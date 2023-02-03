## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:37d568a1e8e46481763223db859dae55eedd4aa86ece9de6f0da7d38e7d6d2a5
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
$ docker pull amazonlinux@sha256:2ae114e4c7fc0532d78268efaa7116b3da72cf053843068ac6e2da54c098f592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390910524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576e65a2c6d2c6a6d838569b1c09d4f95e3f1459e67179429429b373fe2a9425`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:40:07 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a25acb53d1cf2874625ad374a8810cd2ada6730cc44f0118c43cbf60382fd6`  
		Last Modified: Thu, 02 Feb 2023 20:41:01 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
