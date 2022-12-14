## `mongo:5-nanoserver-1809`

```console
$ docker pull mongo@sha256:c8605d213c79a5ede2356b30e1497ff7ba7e8318832ef12989fd16c4449f5bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `mongo:5-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull mongo@sha256:684c1b8c722887455369ffed31b1bf2d11299260a4d43433a688a672b5ac5f78
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416781928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d806d50d0170300aea6506fdf81061fffd0f4fcac240c0a861abfcebbd72786f`
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
# Wed, 14 Dec 2022 01:48:58 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Dec 2022 01:48:59 GMT
ENV MONGO_VERSION=5.0.14
# Wed, 14 Dec 2022 01:49:45 GMT
COPY dir:e35592cc21ade3cccd2a05122103ef64998dd68366a249105c90037f275f3b5b in C:\mongodb 
# Wed, 14 Dec 2022 01:50:33 GMT
RUN mongo --version && mongod --version
# Wed, 14 Dec 2022 01:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:50:35 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:50:36 GMT
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
	-	`sha256:8c002f12039eae15e804c5b2fdfd193fb0622d907f1a5f462d73514cff54e8ee`  
		Last Modified: Wed, 14 Dec 2022 02:25:07 GMT  
		Size: 263.5 KB (263504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d458676cd6f9972b45dd13d00b5d6c80e83f4d0ed5af6e6d09ef36d9c54fb52`  
		Last Modified: Wed, 14 Dec 2022 02:25:06 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefee649f2cb787678e425483137f372480cf70d6fc218f1e8d04168dfe34750`  
		Last Modified: Wed, 14 Dec 2022 02:26:05 GMT  
		Size: 309.7 MB (309692074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6983887bc3b7853ac5417da050787137e9a05d85f0c7b6a244e9c7d8be4059e`  
		Last Modified: Wed, 14 Dec 2022 02:25:04 GMT  
		Size: 74.4 KB (74429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde2cfef94cc7e0ef40bfa9f6fc8a373446bdf14fd1f9080e3bf273629f65f1b`  
		Last Modified: Wed, 14 Dec 2022 02:25:04 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0880ab2175ad4a09747a46d079d0c73cc68f54f9168c2d5f4a43a447d5b86d59`  
		Last Modified: Wed, 14 Dec 2022 02:25:04 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecce33cf275bc0077d39d27290d348871faa5150215bc8fdf0b39a7bbb558c57`  
		Last Modified: Wed, 14 Dec 2022 02:25:04 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
