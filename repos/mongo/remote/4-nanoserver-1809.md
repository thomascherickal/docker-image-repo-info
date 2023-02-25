## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:8a2cfc4881edc3ae9ec2b19bb88dc9b4c43b8b212406eb708539834523b83dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:9843c43a4ab46f4fba5cc84e03a4910c265f35d877a4abc17494301a506827a0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351617593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317e95f355682c99b99ff6067213908fa3f68554a43ff3477b5eb71feb069378`
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
# Sat, 25 Feb 2023 00:29:21 GMT
ENV MONGO_VERSION=4.4.19
# Sat, 25 Feb 2023 00:29:47 GMT
COPY dir:3f48adb7f7619e85ce25694a6fca8d00c40e20a6b52409c21f5809d88aff497a in C:\mongodb 
# Sat, 25 Feb 2023 00:30:05 GMT
RUN mongo --version && mongod --version
# Sat, 25 Feb 2023 00:30:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 25 Feb 2023 00:30:06 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:30:07 GMT
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
	-	`sha256:ba00352baf173332398fb79c9a5ba63ffd45c85f864ae7f611c7062056a71d99`  
		Last Modified: Sat, 25 Feb 2023 02:26:18 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f428901177c869d5481cfdeb5f3c77efe1627b8581687f76a27be08483b49c`  
		Last Modified: Sat, 25 Feb 2023 02:27:02 GMT  
		Size: 244.5 MB (244521659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff88bb751e2d34765912e69d99166d2908914634f9aeb4ea0a1955cfb17cb660`  
		Last Modified: Sat, 25 Feb 2023 02:26:16 GMT  
		Size: 81.2 KB (81196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310b4edfe4305e84ffbe235c9f79d39abb220fc358a4a5baeb6b88eb93bdc0ea`  
		Last Modified: Sat, 25 Feb 2023 02:26:16 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70986252cb2095ede4cd3f89be22ea9ea32845ffdbdd0e1cd28819c55921069`  
		Last Modified: Sat, 25 Feb 2023 02:26:16 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f686752d94412c2553a01cccfe20c83bd1c786f348ebe02462f412e567ec22fc`  
		Last Modified: Sat, 25 Feb 2023 02:26:16 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
