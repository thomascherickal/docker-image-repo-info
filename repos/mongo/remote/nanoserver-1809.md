## `mongo:nanoserver-1809`

```console
$ docker pull mongo@sha256:d2bed2f98b5e32085162111fd984c8eb7d8e7e26d5e449f4163b8d40687e5334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `mongo:nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull mongo@sha256:dddff82bc9d81721d85c0cec8abaae50af3ff9058b5ca9c24dc395b1e689938b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **619.1 MB (619061656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d06c4bca6820e55b666eedcb4029242babc2be191519719c8658efe814365ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 00:31:01 GMT
SHELL [cmd /S /C]
# Wed, 14 Dec 2022 01:37:26 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 01:38:03 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Dec 2022 01:38:04 GMT
USER ContainerUser
# Wed, 14 Dec 2022 01:38:06 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 14 Dec 2022 01:38:07 GMT
ENV MONGO_VERSION=6.0.3
# Wed, 14 Dec 2022 01:39:11 GMT
COPY dir:504ba3c422010154364f85a9b7f5ebcd0252fe3e628d277d138a4248175996a9 in C:\mongodb 
# Wed, 14 Dec 2022 01:39:53 GMT
RUN mongod --version
# Wed, 14 Dec 2022 01:39:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:39:54 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:39:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb1e4df1760e3de08ff30de6fd3f3acf348399853dab1aa1632ed4080cd102`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbb42ac6a3096f2047a475c0c86cb9b35024f73b26ce0e2c0449895724123d0`  
		Last Modified: Wed, 14 Dec 2022 02:18:24 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b83062061825d32cc34037cc0175220e130f9f3d0c86e79ff42affc2376cdd`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 73.2 KB (73169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60417ca99e1256191d2c6e4453104f0c48edc4251a02981488df3a3ce9be5802`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab86ab5b0f077819af56c81822fc89900299552948e62ecb480a6208606f332`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 267.1 KB (267124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ffba1ce258d96e8f9fae90a890e5786c6949e28db2485c631a288c102da1c2`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5628fa0bb535a8309e3119a01e9b826a3a8f703dc3518ee4af5f9ac90937d6b8`  
		Last Modified: Wed, 14 Dec 2022 02:20:08 GMT  
		Size: 512.0 MB (511967875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3af54d20ac81d3432261d13524cd901435d435e43d35ff2178d4af82660b1e0`  
		Last Modified: Wed, 14 Dec 2022 02:18:18 GMT  
		Size: 74.4 KB (74366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6601e0fe68f1aa9d64decdf7c4cd38b70e46e161f0aebd0f665b493d8eabffbd`  
		Last Modified: Wed, 14 Dec 2022 02:18:18 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd743834a96eff3460a81f841d9e25d9cd83046de79c3aea441f675a3c52ef4`  
		Last Modified: Wed, 14 Dec 2022 02:18:18 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c2aa0ceb80171ee8717088d1d8e87f141dfe7e976a7972eb02f549004fc8b3`  
		Last Modified: Wed, 14 Dec 2022 02:18:18 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
