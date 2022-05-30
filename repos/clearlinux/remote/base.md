## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:b40c77884efdb18da1684c07a8c763aab47f6ee53d1a7430a6e82ad4b9ac6669
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:f2da684c1a446b12c14412155851fd170c2d844d4389c2a30b20ab43ffc448fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88141302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899fc31e6c0fc6789e4b4a58ffbcca66f1cccfe032295c2af794505a76565e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 30 May 2022 18:20:23 GMT
ADD file:73abbef5f5f6dbd42f9154201f67a58250748068034ef004b37b147fb11c384b in / 
# Mon, 30 May 2022 18:20:25 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 30 May 2022 18:20:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ac72f30dfc7f6337c7428e168e5489d34882adfbd7334ae399d8efcc2f7bf1b`  
		Last Modified: Mon, 30 May 2022 18:20:53 GMT  
		Size: 88.1 MB (88141084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b5147ed50fd259bef9a9e778c68c1612e1f83e7cc7499eda747300620405d4`  
		Last Modified: Mon, 30 May 2022 18:20:41 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
