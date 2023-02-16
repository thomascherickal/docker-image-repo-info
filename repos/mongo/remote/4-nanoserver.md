## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:490d767433648b96a2a787d28c5ec78f95a3f07406bec1677941224934805d52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `mongo:4-nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:1682e7997addeffcebe6d8b7f8577da9e0dce2ead7b20ab4bde66477d660ed90
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366774270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146ae0df693341045f32b48fa9e1ab74658ee0d4b2c69db0dae8a8824755182a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:56:24 GMT
SHELL [cmd /S /C]
# Thu, 16 Feb 2023 00:46:34 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 00:47:15 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 16 Feb 2023 00:47:15 GMT
USER ContainerUser
# Thu, 16 Feb 2023 00:58:45 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Thu, 16 Feb 2023 01:16:39 GMT
ENV MONGO_VERSION=4.4.18
# Thu, 16 Feb 2023 01:17:04 GMT
COPY dir:f47c837744091598673c1e98795dbb20d206784d286c7f5d0e937f34d552568a in C:\mongodb 
# Thu, 16 Feb 2023 01:17:48 GMT
RUN mongo --version && mongod --version
# Thu, 16 Feb 2023 01:17:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:17:49 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:17:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a1068ea860cf7cfcf2570b406077f352946c2ab4e7cc47dafeea0ad296184c`  
		Last Modified: Thu, 16 Feb 2023 00:29:48 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db214e24db987418d45852de020b518bd1f2775c39acd283d3dc32a2d43a9cd2`  
		Last Modified: Thu, 16 Feb 2023 01:39:07 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a09543181ef38cc231e4c1aeaa8c3659c87805f41b3aa4de1846f7ecafaa5d`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 83.3 KB (83288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778f9c80c9fc406ad9bd5c358bead14d62b3e09a69819cfd63b1fca3591c648f`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f94424346605341414054d10c35e3985dc7612a4b4ea3915e3a7322bc2ed864`  
		Last Modified: Thu, 16 Feb 2023 01:44:29 GMT  
		Size: 263.5 KB (263520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe6a0097590418fbc3bd8ab86e93103cb5771eb46ebc3fbba68bd2f720958b8`  
		Last Modified: Thu, 16 Feb 2023 01:52:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e8b7903b8860ead1189b6bb359a86c50644db2814cd4a1771cdafb4dafabfc`  
		Last Modified: Thu, 16 Feb 2023 01:52:52 GMT  
		Size: 244.2 MB (244246852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104ae153d215f773cc8e1526c667441ebd9343bbeb25608801dc8ee75c775f3e`  
		Last Modified: Thu, 16 Feb 2023 01:52:08 GMT  
		Size: 53.6 KB (53578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5ba56c1a4f4c4fab29b400c9b6053662ee18410b263672da72633b23223ca0`  
		Last Modified: Thu, 16 Feb 2023 01:52:08 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e556692d97022ec804d797b7d3a5244459428a0db93c41d8f09eba831baa1`  
		Last Modified: Thu, 16 Feb 2023 01:52:08 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc43a3e312d45f01d53195098c9369d0d81945b461f27dc7ea95203d5038b96`  
		Last Modified: Thu, 16 Feb 2023 01:52:08 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:6aaef5774d20f26fcff30b86afecdf3fbbd4bf2fff15831638944285cc9d01c2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351344351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa37033af1ddb11d4db64d713902749f16d7ecf9b6547af6f9ec57d3f2c44d36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Thu, 16 Feb 2023 00:01:27 GMT
SHELL [cmd /S /C]
# Thu, 16 Feb 2023 00:49:20 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 00:49:55 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 16 Feb 2023 00:49:56 GMT
USER ContainerUser
# Thu, 16 Feb 2023 01:00:15 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Thu, 16 Feb 2023 01:18:09 GMT
ENV MONGO_VERSION=4.4.18
# Thu, 16 Feb 2023 01:18:34 GMT
COPY dir:f47c837744091598673c1e98795dbb20d206784d286c7f5d0e937f34d552568a in C:\mongodb 
# Thu, 16 Feb 2023 01:18:58 GMT
RUN mongo --version && mongod --version
# Thu, 16 Feb 2023 01:18:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:18:59 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:19:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e6d0fd50a58d89dbedba25508f81ef068969a7464dbe7797043bb469eede73`  
		Last Modified: Thu, 16 Feb 2023 00:30:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5eddc7e8d799a6d70e3c7af26d160bf2b4d8b64941a7060be52fdeb0b79acd`  
		Last Modified: Thu, 16 Feb 2023 01:40:41 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a259616c0c928b5b30118ca22d90192b5d9737f409fa661516b4f49b37a818f`  
		Last Modified: Thu, 16 Feb 2023 01:40:39 GMT  
		Size: 68.9 KB (68858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd33c33cfd9a8bfca2346ed26b9aa877be5373eaef63050cfffbc28069e192`  
		Last Modified: Thu, 16 Feb 2023 01:40:39 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21ac80a5938f2f6793901c9505c1317c3d32ed634405e21b653a4f3b3f6fc8f`  
		Last Modified: Thu, 16 Feb 2023 01:45:36 GMT  
		Size: 263.4 KB (263413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ef984c4fe70a1ca19948f2f132e81f54820b8f7d0718a8d4b19e256fbfbe97`  
		Last Modified: Thu, 16 Feb 2023 01:53:06 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977def503e06d9372a2395db6678a305a1bebadbea0ee8cfd246d9a2c8b138d2`  
		Last Modified: Thu, 16 Feb 2023 01:53:49 GMT  
		Size: 244.2 MB (244246878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60748c3691adcccb73505add0c56e806b74322ed5d0a4818df7d7bbe8805254c`  
		Last Modified: Thu, 16 Feb 2023 01:53:04 GMT  
		Size: 82.3 KB (82310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec77f53c56fd27657df66252b5ac9dfc2ac60da5b626ceb7c72d40381672960`  
		Last Modified: Thu, 16 Feb 2023 01:53:04 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d66cc3b8cf9fe9bd530b4fe41346b671f3fad3d84b06a85565d1ee1831f3874`  
		Last Modified: Thu, 16 Feb 2023 01:53:04 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea204d1fac43115b9be3d1ca29281c24f502eb30a9aa369f05be4fcbec84f93f`  
		Last Modified: Thu, 16 Feb 2023 01:53:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
