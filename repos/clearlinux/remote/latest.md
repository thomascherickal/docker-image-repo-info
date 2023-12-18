## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:210604f3a737df47c6d83f78c54ee7da6b2f82fee0d08ad40b48af1d4850a3f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:d97e401e847fa930ec0fc2741bbf537e28be30a816098f876c7b5b5ba49505da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68054799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085319036821156c9b07c86f5f5006c8a987e8756b4fd1e77b87c04878584f22`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 18 Dec 2023 18:32:13 GMT
ADD file:23a2cb54909cfa9a4483475458c5c5a54863e3c2bd8b84c86ece9f0c7416bd16 in / 
# Mon, 18 Dec 2023 18:32:15 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Mon, 18 Dec 2023 18:32:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7c63dc98be1b3290f53818352c82d6da61f0ca6633ae8bd6fc7362fe62d522f6`  
		Last Modified: Mon, 18 Dec 2023 18:32:45 GMT  
		Size: 68.1 MB (68054586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd98a7424503368773b6644a8a25c5aa3bab61f414dedb8faf1dc6c12a9cac7`  
		Last Modified: Mon, 18 Dec 2023 18:32:36 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
