## `debian:experimental-20221219`

```console
$ docker pull debian@sha256:2c2ab04a23d8715fa9b956bf00347b14b1a51cf478415dc2b05f25e70f0db8d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; mips64le

### `debian:experimental-20221219` - linux; mips64le

```console
$ docker pull debian@sha256:f9e06349289968e72b817e9fc0511a6059db60d427232035483bc8059c0f0fea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50293171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75a28d29ae62f6c840a5af603020882890c8196a724cb963db47c3805b6d22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:14:36 GMT
ADD file:d86f0e28d7ea72ca80aec16cc53a8efebf43b4802fbbed1b6452a0730f13e73d in / 
# Wed, 21 Dec 2022 01:14:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:15:19 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c1a8c1357338f60ee5392f4bf29f089ea8ef5e17f25a0a3f49fce091aebf025f`  
		Last Modified: Wed, 21 Dec 2022 01:23:08 GMT  
		Size: 50.3 MB (50292947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20db7e5faa75df970592e05e4ee9d6d361a077f5366dd189fd1c1647b5386cc3`  
		Last Modified: Wed, 21 Dec 2022 01:23:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
