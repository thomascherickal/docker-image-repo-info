## `photon:latest`

```console
$ docker pull photon@sha256:a2896b917eae977c8e844fc8060a23ea286bab6da27ae12a48b538feb931517c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:efccad65228d06c86fc69abf5eff218f3add1e9bf5f787bd284cb54a28e0e1eb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15124940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f28e659100054bd3b2cbabd44504a37aec6af865c7a874335c50cea3221c060`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 17 Jan 2020 23:49:17 GMT
ADD file:8be68d07e8ce26981d81c179437e451449338092faec4ad96241aac2ecdf62f7 in / 
# Fri, 17 Jan 2020 23:49:17 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200117
# Fri, 17 Jan 2020 23:49:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:28d1a3c45ca766655b9bb7bf9509318b529bf15176ae236c364cd062472179e9`  
		Last Modified: Fri, 17 Jan 2020 23:49:58 GMT  
		Size: 15.1 MB (15124940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:824edf39334d799baccadd18e86c7d38253b51908769228cf6e5bae6b681a9dd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12939483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36433f5286adeebc892f51f9cf3c738bffc1f8903a1ce0f9dbbfc6384ff66964`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 17 Jan 2020 23:11:06 GMT
ADD file:267145652ff8b22e3ffa2c705dc322aa77a5811f09cb2c8af3a2846086e683dc in / 
# Fri, 17 Jan 2020 23:11:07 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200117
# Fri, 17 Jan 2020 23:11:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c5072a4ac61960021f6bd887ac01b785422c29bb071b97889facbe827ae114f9`  
		Last Modified: Fri, 17 Jan 2020 23:11:30 GMT  
		Size: 12.9 MB (12939483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
