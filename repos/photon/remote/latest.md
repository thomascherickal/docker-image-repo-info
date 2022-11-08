## `photon:latest`

```console
$ docker pull photon@sha256:90abe1fbaae8181c9b7599d4b6a6274f98d144387fbc0ac73c272b09b59efbd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:2cd164c41dc73b8f7fc4cdee163d7ffc9cd7ebb12a96e179dded8006ecf36d8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16076347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc45c395fa80a4953809f627fc75df93f399c5f84058a95639f86ef9713204f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Nov 2022 22:32:56 GMT
ADD file:1c334dd0bd0c614737936c6cbfc011cfdea28b70c75abd2615f808b44c239dab in / 
# Mon, 07 Nov 2022 22:32:56 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20221105
# Mon, 07 Nov 2022 22:32:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d46c4d5563bcfe534e24a4a89cb29f8295b62e56996cfed24a2b0da3ec251866`  
		Last Modified: Mon, 07 Nov 2022 22:33:15 GMT  
		Size: 16.1 MB (16076347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:2b6f826e7e98735d0bdd2deb6bcbebde98bbecc6c02779d2d753da2dfc75fddf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15161398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa22972c75fdd36e93e92b8e826858528c085f06cbffa7be19e3105d670633ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Nov 2022 22:37:40 GMT
ADD file:9cb23d6d3d25edda5131d3227ffa854da7b48f278fb7d4ed7d990d38e1b2b895 in / 
# Mon, 07 Nov 2022 22:37:40 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20221105
# Mon, 07 Nov 2022 22:37:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97aabc8583fc02f3f2b18ea25e1d2c71e2f80ce6efbcb41e4cf33b6a33578a65`  
		Last Modified: Mon, 07 Nov 2022 22:37:57 GMT  
		Size: 15.2 MB (15161398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
