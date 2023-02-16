## `mongo:nanoserver`

```console
$ docker pull mongo@sha256:1edfbb23092bf171a66de1da29a79a3d9a9189ff03730233cc649d268f70d986
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `mongo:nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:5e58a37e1cdc56f9f2a4cff08667d0d99fa790a1cb61509c72eaa591b66175cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **634.8 MB (634803301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de229985a9fcab3cb5bef7a8ed5164b9aa86f9b97fd281ce71961a3b4774514e`
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
# Thu, 16 Feb 2023 00:47:17 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Thu, 16 Feb 2023 00:47:17 GMT
ENV MONGO_VERSION=6.0.4
# Thu, 16 Feb 2023 00:48:17 GMT
COPY dir:68661c9bc66199176f558318104ff5aa0937d5a9cd22b931af66fda7826a6f78 in C:\mongodb 
# Thu, 16 Feb 2023 00:49:03 GMT
RUN mongod --version
# Thu, 16 Feb 2023 00:49:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 00:49:05 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 00:49:05 GMT
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
	-	`sha256:a6c5820762c82f2d8598cdfeec5c188618393712d380c457660230a1e49c1cda`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 267.1 KB (267067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726394b332b54f08d080ed6d531077a9aa912bc7925c66e6c80e6d2cca118b16`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487a5e0a0046226bc59b5cc407c024e8eaf658676c1b0cccb5ca02051cabab2e`  
		Last Modified: Thu, 16 Feb 2023 01:40:22 GMT  
		Size: 512.3 MB (512272743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e94b9b64c41c911d396795d37900874b2bc6e20f37e85718c885b1b5d6ce476`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 53.5 KB (53537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4419b89d5de3688e8bd8adba7cacd26a6a8f4ad212d2294c1983afeb8cee45`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefcd5351c904a37071c1cf60ffcf5c13543205c48772492ddd734d33abfb231`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bb3202fd2aa02d048c45b682f76cb1af285fc79d28c85f1d99e52f3cd429db`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:d07612d37ae37b77f1a41aaead4c766177973a25a3db8d1b9a1b88cc6620a629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **619.4 MB (619374946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0ff02f5bdc3837f0f071fc3b777c7218e0183237bc02b7f5d1be48eb4b6c7b`
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
# Thu, 16 Feb 2023 00:49:58 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Thu, 16 Feb 2023 00:49:58 GMT
ENV MONGO_VERSION=6.0.4
# Thu, 16 Feb 2023 00:50:55 GMT
COPY dir:68661c9bc66199176f558318104ff5aa0937d5a9cd22b931af66fda7826a6f78 in C:\mongodb 
# Thu, 16 Feb 2023 00:51:29 GMT
RUN mongod --version
# Thu, 16 Feb 2023 00:51:29 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 00:51:30 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 00:51:31 GMT
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
	-	`sha256:1d83a0f62ae6c23d5f01f60c2ecc9f4eb1493ddc8fae583639608f57cc96a70c`  
		Last Modified: Thu, 16 Feb 2023 01:40:39 GMT  
		Size: 267.0 KB (267040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd5143baf40e62f0ffc7051554c43ba921435c36655422dd8a8f325b5f00001`  
		Last Modified: Thu, 16 Feb 2023 01:40:39 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc9634a2b8d1d5d24b7351ec53690fce5d7a297d9bcdc8b2269f2e16250622c`  
		Last Modified: Thu, 16 Feb 2023 01:41:57 GMT  
		Size: 512.3 MB (512272087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e3ed9f2ad553c83c862c35473161ba519c07f9b1914708ce2ad5bd770d8668`  
		Last Modified: Thu, 16 Feb 2023 01:40:36 GMT  
		Size: 84.4 KB (84407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f1824afc725d3a6ec190aabd6debd65019deb0654f3e7f6135aaae8fc008a`  
		Last Modified: Thu, 16 Feb 2023 01:40:36 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bace6598b496f42e81d2bdd5ff81e570a2dd3f068403f85839c9e5c0ea6fa679`  
		Last Modified: Thu, 16 Feb 2023 01:40:37 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc69bb21fc3c83431efc66c6e5657d30a0509a5acbf133de49ce2d5ca738b88`  
		Last Modified: Thu, 16 Feb 2023 01:40:36 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
