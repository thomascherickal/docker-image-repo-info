## `mongo:nanoserver-1809`

```console
$ docker pull mongo@sha256:98c708f204f759d3a1469c0f63a2d3bbd66eaeea1a48a81de1247acdeaf5eaf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `mongo:nanoserver-1809` - windows version 10.0.17763.4010; amd64

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
