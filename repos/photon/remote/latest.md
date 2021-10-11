## `photon:latest`

```console
$ docker pull photon@sha256:0a4bbd988b1b3f8a61a6364d68d4ba71e1b924066b37d7a0022023b7f188e57d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:bf8386fc78687980e7a7075760c8ea7496be62ef0644c66e3cd3cbffa2b6b712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15971580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cc42b8571fae499eb9b3315a407d91ac265ffd3307dc9931e0c63d2fe896cc7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 02 Oct 2021 00:20:45 GMT
ADD file:a664c1e62a5272618a5894ec88e2ba95871882c0567ce8a84c4fc75530f7daad in / 
# Sat, 02 Oct 2021 00:20:46 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20211001
# Sat, 02 Oct 2021 00:20:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1ca17a650be2a92afd2e9d4f70289672b13f34592e10ed45512264f1173071fa`  
		Last Modified: Sat, 02 Oct 2021 00:21:56 GMT  
		Size: 16.0 MB (15971580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:71089b4682fe07043b2ed400fb1145c6e2496df53445b101f350ace2d93b8695
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15003365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7cda01197939a6af097037427db930bef0420f1704288ff8955d67603f35d8a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 11 Oct 2021 17:39:53 GMT
ADD file:c6a96f727a865badc73162b592c8499bc0107beb0540727bd482c7e67982a359 in / 
# Mon, 11 Oct 2021 17:39:53 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20211009
# Mon, 11 Oct 2021 17:39:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2681d12baac3d93408bcec5ef56814be0cf053dc94159b25c1968b5ab272541b`  
		Last Modified: Mon, 11 Oct 2021 17:40:23 GMT  
		Size: 15.0 MB (15003365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
