## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:dfd5418b6ec0e1fe2851a654aff4d4af767bb410cbf53933a17009b861864baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:74b3d4f1c67eeb58c4e6541044bb2d57098615775090c14089451a5d1295ce5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68818941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d4c3e03d4f628025cd0fe135051fbcf7085773876e6eb8718fc52b56997a86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 24 Oct 2022 21:23:41 GMT
ADD file:08412929066e10427fc1d228d4802e49f5d4c51ad62ce7143db789c45dabd49a in / 
# Mon, 24 Oct 2022 21:23:42 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 24 Oct 2022 21:23:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:90a9fa5bbdc5d22fef360f2eecc8c887d1c9c74b01cd7f472fee57146a8e2a94`  
		Last Modified: Mon, 24 Oct 2022 21:24:01 GMT  
		Size: 68.8 MB (68818723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af46fc9ddd5c4f45b066cab4b0628a4b8dbd0a165a9ee224585d812dff6562e`  
		Last Modified: Mon, 24 Oct 2022 21:23:51 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
