## `archlinux:base-devel-20221002.0.91257`

```console
$ docker pull archlinux@sha256:5661abc584c522c46ebf99a12f501703a36fcdfdd9f4953c2cd5b50125abc1dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221002.0.91257` - linux; amd64

```console
$ docker pull archlinux@sha256:2fc3c860b6e61f9759eeaaa4542c429dd8195479da82334bd1509c32fb1886b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238593146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420395b56c93b0fadae42e2f4424e3e4b474ebafd74b486fa59193bd02073f80`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:20:58 GMT
COPY dir:18fea0b266ee182d9d39f5c46c96dce2236a702069f997545d0df7b9c4099d49 in / 
# Mon, 03 Oct 2022 21:21:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:21:01 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:21:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:a64de180eba4662e4ee754ae56002a9e7471e8f9a44f207562a29b6beacd97aa`  
		Last Modified: Mon, 03 Oct 2022 21:22:29 GMT  
		Size: 238.6 MB (238584575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c4e6705d653db25362d4666e5e9cdbec07661b7974c69350629df6a01de0e`  
		Last Modified: Mon, 03 Oct 2022 21:21:54 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
