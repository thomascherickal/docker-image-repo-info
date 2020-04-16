## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:ca50d9e3d89ca27290f5590ee2f44045905a33ea3b089ea751a981e88f71868a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a3195ff738fa58d110f2178088e551cedd6f55d4c6bf5fba6e79a923b7d3fab4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71936652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d4aa31cbd8bf22629c7e10e54f38ae51f2aa9fb970a299ba47d5f5c2f96aaa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:07 GMT
ADD file:06c434cd627b8970a4f3d8d76b36955fbf53b74db3f0ce29f1fc3b269c81f2eb in / 
# Thu, 16 Apr 2020 03:23:08 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:04:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3707da5d661028328ae23959ded4ecbb1e5ddbe2a4e8551cd5b6f90e90e6cbd5`  
		Last Modified: Thu, 16 Apr 2020 03:32:06 GMT  
		Size: 54.4 MB (54390842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a013c08ba606e93a8e6efa446e68ae82873c251f8d211d99fb2c3896cd7df989`  
		Last Modified: Thu, 16 Apr 2020 04:17:25 GMT  
		Size: 17.5 MB (17545810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:494a3a6be629bfcd17272fe7852c38e4df5cad9b2773698f166f74583fe107e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69617295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bd6b8d386bd1848cf6830ee33d1693bb4f0ec8fe920391e40abda1a12de731`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:25:13 GMT
ADD file:631f76030613657eb3d82228323e5a3860b5141b58858b628bee342bd47d427d in / 
# Tue, 31 Mar 2020 01:25:17 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:29:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:29:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3ebddd0cca47bf5452de875b55a7b0a10e182a550196df63972f211a03e9f7cd`  
		Last Modified: Tue, 31 Mar 2020 01:33:28 GMT  
		Size: 52.6 MB (52580205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e80167505cea44898f4dce8e6007acae3e6ccf8b0b3b62d514cb4d769474d4`  
		Last Modified: Tue, 31 Mar 2020 03:48:54 GMT  
		Size: 17.0 MB (17037090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f31c39b5fd7515bf0db51301f4f19eb199fe1bec9afe07fe7d75ad0e0fb38079
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67027664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da1b237044f964087658b9d80398029330908ef6d82ebddc93f9777eaf2bd4c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:00:13 GMT
ADD file:0b08b600835a16058b725946cb7ae338fea6a14cf6998584f9728d2c62324f1e in / 
# Thu, 16 Apr 2020 01:00:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:44:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cc084eacfbe394e053f99559ca63f9d660d60dad0b70a31347e5088af534b2e9`  
		Last Modified: Thu, 16 Apr 2020 01:09:20 GMT  
		Size: 50.3 MB (50304312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2753eba5d276059ffd460d19c6e651040079c4a18c7d6a93682bef3e285c0b9`  
		Last Modified: Thu, 16 Apr 2020 01:58:21 GMT  
		Size: 16.7 MB (16723352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:052787992f53a811092c7976a0e74790a1b84837bb2e94bedd894e8b0a14e2d8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74463685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de3400688e4ef0e7e8f85aa5f58ff988641270e5408546e05a717664aaf6f0e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:40:13 GMT
ADD file:fc5ade2a561dca01c2a4d4035601db636d098801b5655a1bf239e8b706395f87 in / 
# Thu, 16 Apr 2020 01:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:23:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:582c227f31bedb5a1092c02e624ef551c8659052150d9e9368da891fffd1528c`  
		Last Modified: Thu, 16 Apr 2020 01:46:40 GMT  
		Size: 54.6 MB (54607914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1866a4665d6ee342c90adf77b23d7002ec3ef1fc701d3c2df2ca95ab860994`  
		Last Modified: Thu, 16 Apr 2020 02:38:43 GMT  
		Size: 19.9 MB (19855771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
