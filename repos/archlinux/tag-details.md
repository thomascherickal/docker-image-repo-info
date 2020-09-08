<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:20200908`](#archlinux20200908)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:20200908`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:e543fcbafadece75d0129ac04484b1cb2c36c18847c8609ae7634fe11c688651
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:ce7ccce2c458b875f66a0e33d492ccc2f5495dbf21a7fc9acd261f8f980d4fd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129593465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5dd8b4c81531625c5a31cf082aadf1af8348e34f9183baecdca000ef9165373`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 19:20:08 GMT
ADD file:94b9927b243c82b2ea4201cba2528f25207a52c64624ce8abe4dd0e599dcd75c in / 
# Mon, 06 Jul 2020 19:20:12 GMT
RUN ldconfig && update-ca-trust && locale-gen
# Mon, 06 Jul 2020 19:20:13 GMT
RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/systemd-hook sysusers '
# Mon, 06 Jul 2020 19:20:13 GMT
RUN ln -s /usr/lib/os-release /etc/os-release
# Mon, 06 Jul 2020 19:20:24 GMT
RUN pacman-key --init && pacman-key --populate archlinux
# Mon, 06 Jul 2020 19:20:25 GMT
RUN rm -rf etc/pacman.d/gnupg/{openpgp-revocs.d/,private-keys-v1.d/,pugring.gpg~,gnupg.S.}*
# Mon, 06 Jul 2020 19:20:25 GMT
ENV LANG=en_US.UTF-8
# Mon, 06 Jul 2020 19:20:25 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:52d0bcceb754dd7a78cbb36bc96eb7a5da104f072f878425d4faec10d024decb`  
		Last Modified: Mon, 06 Jul 2020 19:21:34 GMT  
		Size: 126.2 MB (126232079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b70b20651854b1ed8814d07ef050c9f7a9b3ba01a810dfb0beabaa3c85244c4`  
		Last Modified: Mon, 06 Jul 2020 19:21:10 GMT  
		Size: 1.6 MB (1584430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e55ff511d01b60faaa676d53e4bb621c7b973c720d18f2bc18d317119c121b`  
		Last Modified: Mon, 06 Jul 2020 19:21:10 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f632385a0cc2af80952b4c26014fcb8b9919e43fbf67e48d73c8c95f63c739`  
		Last Modified: Mon, 06 Jul 2020 19:21:10 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6fe943aedd0944fd91b12da72ff449b9697645abd3e11f1eec91420f6e798`  
		Last Modified: Mon, 06 Jul 2020 19:21:10 GMT  
		Size: 1.8 MB (1775397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482970d479e41eed6b2cae87b93c1c57e02fd449e717ae228ac661f380c03c26`  
		Last Modified: Mon, 06 Jul 2020 19:21:10 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
