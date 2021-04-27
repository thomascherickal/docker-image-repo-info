## `archlinux:base`

```console
$ docker pull archlinux@sha256:fc2d451eb32bbea6e4eb784108b61cd8c109c9ad9ddfd1253e9984533836c592
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:d141bed664f15850272a691bc1f547d518ed3aa1bb91b6c07ceb0d0efb37959f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134669556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c54ea3314ad37f90930832757897cdcfca0d66c93471883fbc773ac58a13fadf`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 26 Apr 2021 19:20:12 GMT
COPY dir:af5a52e0bbc7f1eb1783bcf0f24f4156358f219c4562dd27db7663db3d053d7e in / 
# Mon, 26 Apr 2021 19:20:14 GMT
RUN ldconfig
# Mon, 26 Apr 2021 19:20:14 GMT
ENV LANG=en_US.UTF-8
# Mon, 26 Apr 2021 19:20:14 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:2ed5206556418c02f5f803f04e9e250fee51e76338d7edac1904569731a87645`  
		Last Modified: Mon, 26 Apr 2021 19:22:01 GMT  
		Size: 134.7 MB (134662915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71981185e000c6639920765540f7562a71649a09d94573b1158fa3dbadaeb112`  
		Last Modified: Mon, 26 Apr 2021 19:21:41 GMT  
		Size: 6.6 KB (6641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
