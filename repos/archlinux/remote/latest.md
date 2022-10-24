## `archlinux:latest`

```console
$ docker pull archlinux@sha256:71df376dbf28d6eaecbe9de04e394566afeba74e8cac2b2fdf36e05c5ae0b1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:bc4ed3be8c243364fcd35efa1c0453a60656273a503db678bfb539636e9faa64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140617937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07c50d60718b29af087862ef10d0652f308738ba62d3ff0c76fa904c1a75c0e`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:20:00 GMT
COPY dir:4752ae61421385c24c18856c8a2557961ebd3b1a21b1a47b5c4e9b945445c0c9 in / 
# Mon, 24 Oct 2022 21:20:02 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:20:02 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:20:02 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eebb07dfd16c7bf2df5098fe297270d6244a762136b62f00439a1f93b8efd904`  
		Last Modified: Mon, 24 Oct 2022 21:21:46 GMT  
		Size: 140.6 MB (140609989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2ee4e22db4ca78665baa96d081d15e1e49bd99bb86a15bd8314535db437b1a`  
		Last Modified: Mon, 24 Oct 2022 21:21:25 GMT  
		Size: 7.9 KB (7948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
