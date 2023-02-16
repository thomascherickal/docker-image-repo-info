## `mongo:5-nanoserver`

```console
$ docker pull mongo@sha256:2aeb602a37122b5bfa762337e521940f65ab89376890974764c2951699466e5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `mongo:5-nanoserver` - windows version 10.0.20348.1547; amd64

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

### `mongo:5-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:612cbe0f6ea2d735c72481adf7114213b5fc3efdeb1f6a22b5307db798a4c5ed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.8 MB (416793912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:710e8c10277576a07607ff06824bbdb5f2b889ccdaefa1553ecbca29fdd8dd86`
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
# Thu, 16 Feb 2023 01:00:16 GMT
ENV MONGO_VERSION=5.0.14
# Thu, 16 Feb 2023 01:00:51 GMT
COPY dir:e35592cc21ade3cccd2a05122103ef64998dd68366a249105c90037f275f3b5b in C:\mongodb 
# Thu, 16 Feb 2023 01:01:28 GMT
RUN mongo --version && mongod --version
# Thu, 16 Feb 2023 01:01:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:01:29 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:01:30 GMT
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
	-	`sha256:33ba65d81594858668b6a5ba1345091c8b619f69fb08fd77e89550a8eb4c80ba`  
		Last Modified: Thu, 16 Feb 2023 01:45:35 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6b5c1f5e611253ae1046fd2905265518686f088e84eafd5fdfa7fe82268508`  
		Last Modified: Thu, 16 Feb 2023 01:46:29 GMT  
		Size: 309.7 MB (309691930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9676048cb5bfa3d17d61c51ce14a5411237e0e2fcc2e3d5266071d4cfc92471`  
		Last Modified: Thu, 16 Feb 2023 01:45:33 GMT  
		Size: 87.2 KB (87204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9197c6a82b51a5ed4a297b3a62d3e2111ea02921efa99fa64f48edc300abe945`  
		Last Modified: Thu, 16 Feb 2023 01:45:33 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97cf7b3a38b553b7a87a5fe841b80755bfc74baaf7aeaa27cb8b3908f038534`  
		Last Modified: Thu, 16 Feb 2023 01:45:34 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75535517a7df5d77536c538de0b22eb7b53840b7841f0b0cb83bf431a7cd27d8`  
		Last Modified: Thu, 16 Feb 2023 01:45:34 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
