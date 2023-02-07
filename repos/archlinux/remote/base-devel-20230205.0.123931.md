## `archlinux:base-devel-20230205.0.123931`

```console
$ docker pull archlinux@sha256:ae4a80a09f6c759676a038fbaebc3f744c0dd23dd01e07b4dd6edfb78a35f237
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230205.0.123931` - linux; amd64

```console
$ docker pull archlinux@sha256:16205ffa58aab2b975467fc59d4acd4f21558da458f54fc535fe37a81806cfba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243487052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c550d9031f67c135c6dd9154a5f2afd924d0b859b4a6f5877c54a7b4de4fa66`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:22:38 GMT
COPY dir:9be8ea933917715fc38c864b797a6ce33209be32699cc7148344c74148e398d7 in / 
# Tue, 07 Feb 2023 01:22:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:22:42 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:22:42 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:fe3c997a2b8a77cf9c9a7a5f8f1dec6d51f9d2330c7e8c73bf0f83681669ba58`  
		Last Modified: Tue, 07 Feb 2023 01:24:07 GMT  
		Size: 243.5 MB (243478410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab90887e196be5bd981c542b642511ab3735e28591beebab9671155c559062c8`  
		Last Modified: Tue, 07 Feb 2023 01:23:31 GMT  
		Size: 8.6 KB (8642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
