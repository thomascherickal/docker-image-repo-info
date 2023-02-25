## `mongo:5-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:5dce683eddf00b31a2bd04a28f4c1590ad42dac07ab2b2721edf83adb49337b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `mongo:5-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:75456f77ec013f8b7893a4a1b00995eb4bbb6d08e93ba45e5bcc40a61930649d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.7 MB (433659212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f72455e6f7b853d3af2d1ac1cbb117c60f8c3e8340ec79eada5900e4fad55942`
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
# Sat, 25 Feb 2023 00:21:11 GMT
ENV MONGO_VERSION=5.0.15
# Sat, 25 Feb 2023 00:21:43 GMT
COPY dir:fb2387548719c31821557ec72e326693578135a8ffa29c575b7481c4a733db86 in C:\mongodb 
# Sat, 25 Feb 2023 00:22:01 GMT
RUN mongo --version && mongod --version
# Sat, 25 Feb 2023 00:22:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 25 Feb 2023 00:22:03 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:22:03 GMT
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
	-	`sha256:295f951f42efbe30270e0f6954c142717ea808ca85049b0bc83ec58dca6a7823`  
		Last Modified: Sat, 25 Feb 2023 02:21:04 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555ab072a78d63ffa09e668929c31ac7ceb1cf350d7c38db2e2ef6f1b9808f4d`  
		Last Modified: Sat, 25 Feb 2023 02:22:03 GMT  
		Size: 311.1 MB (311131558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562953072e67f1b0c22070eac69872f4c9b45edb38277e14fe92ce678d951602`  
		Last Modified: Sat, 25 Feb 2023 02:21:02 GMT  
		Size: 53.8 KB (53805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92e17ab1cccd982df446d4dbc84fcc582d0909138338e71f551a865e64fbf26`  
		Last Modified: Sat, 25 Feb 2023 02:21:02 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7696ec9e07f01c79fe86b372bce8f8211ea1172fb15a24244700ec0179be680a`  
		Last Modified: Sat, 25 Feb 2023 02:21:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2b889ddbc41ae7718e4da3e61f24feee9d967a69d959763d89f11677dded95`  
		Last Modified: Sat, 25 Feb 2023 02:21:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
