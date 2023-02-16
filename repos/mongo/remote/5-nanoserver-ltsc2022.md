## `mongo:5-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:539aabab27ca08fdb2eb2abf3f043077d86c95bf0b8da7be3068886fd4a8e8b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `mongo:5-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:237f73cbfedd2d13ca84f6f8ff457a745b3b1ddf84b2c7ae99f7ca79f0ecae85
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432219120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aeff7cb67e336a7c3abd93a7c0da3524823525f6bf8c3921476d290688cfdc3`
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
# Thu, 16 Feb 2023 00:58:46 GMT
ENV MONGO_VERSION=5.0.14
# Thu, 16 Feb 2023 00:59:22 GMT
COPY dir:e35592cc21ade3cccd2a05122103ef64998dd68366a249105c90037f275f3b5b in C:\mongodb 
# Thu, 16 Feb 2023 01:00:02 GMT
RUN mongo --version && mongod --version
# Thu, 16 Feb 2023 01:00:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:00:04 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:00:04 GMT
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
	-	`sha256:d4a656155b8e79652270b521bc4586845dfb98c050d008f6e110ad2d44c36676`  
		Last Modified: Thu, 16 Feb 2023 01:44:29 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7dcf74d7373c93c1042f935d1774cf77d845ecda15bdc51f3e19f04e9fe3de`  
		Last Modified: Thu, 16 Feb 2023 01:45:22 GMT  
		Size: 309.7 MB (309692142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eaf3c6a73cd61c09922eca146bc029e64f06c9d341f382e37421895be7752b`  
		Last Modified: Thu, 16 Feb 2023 01:44:27 GMT  
		Size: 53.4 KB (53445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ed615ce9f51fbb39cd3899157b338bfb9a0834fb4e407030e3ab3453a09abf`  
		Last Modified: Thu, 16 Feb 2023 01:44:27 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66799f30d4e206ee07177cee04841fc44d21bf4ccdceeb65d3ff8ca730c30881`  
		Last Modified: Thu, 16 Feb 2023 01:44:27 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ec0e1fbe528d1a942dbdfe47a8b8dd12e1879df5fe2beb51e19c509bb3cc5`  
		Last Modified: Thu, 16 Feb 2023 01:44:27 GMT  
		Size: 1.0 KB (1013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
