## `debian:experimental-20221024`

```console
$ docker pull debian@sha256:f1b0b54c1caf115e76858fbe5f396ae748eaeb40b2ee342e46f315124d5a1075
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; s390x

### `debian:experimental-20221024` - linux; amd64

```console
$ docker pull debian@sha256:154fc729cc812cedeeca8446d15d9e344067e351aacf4856156c218bf0e835a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50641427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:061216c4987060efde1cba818de03f256d65af769f5e0c726c47e3cee89519d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:45:38 GMT
ADD file:1547e086dc40d3418e8f146e3b7fe2141ad7659675f0a810d3723f618ce685f3 in / 
# Tue, 25 Oct 2022 01:45:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:37185fef75d9c859c0943d1efbb25a8ccb6052762fdece7628188b1dd148c6b2`  
		Last Modified: Tue, 25 Oct 2022 01:51:27 GMT  
		Size: 50.6 MB (50641207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187a9a9e5cbb08d19f59ebb1026adfa6311b7d5962ee3eb8789bf89adea76029`  
		Last Modified: Tue, 25 Oct 2022 01:51:49 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20221024` - linux; s390x

```console
$ docker pull debian@sha256:3696bfecd4373574428052be1c6bc57f86857903acb5c6b86fb7b0ae9031fb86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49013157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b736aeeda8a8eee6fc99797030aedd3efd0c0f0c53950bbb63d4993259e6f5bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:16:15 GMT
ADD file:0258dcf1ca7bf72abeb6bb2a139a712f118544a38e38c277acaae984d4312e12 in / 
# Tue, 25 Oct 2022 01:16:17 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:16:34 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ad8b0151e3d93e0406fa9194bfc8fabf5a340300bed913637542073f2f8b0eb8`  
		Last Modified: Tue, 25 Oct 2022 01:20:42 GMT  
		Size: 49.0 MB (49012938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bb1bf872871a010d0b98d4063c2111eaedaa5837abc609668142bdd837da14`  
		Last Modified: Tue, 25 Oct 2022 01:21:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
