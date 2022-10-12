## `mongo:nanoserver-1809`

```console
$ docker pull mongo@sha256:8418ccdd7acb304c93cc2d7f2be0bb520bad42213365641cc1a7c070b095033a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `mongo:nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull mongo@sha256:0a45979162b304c9fafb18592c44b3f2ef4a28c647a39921a1177a7ac2fedff6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.2 MB (615161620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e377af73e20e75948596b83a675d7a7cd7c84f3df2fec0435c47e166e3d399b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 12:55:53 GMT
SHELL [cmd /S /C]
# Wed, 12 Oct 2022 17:14:20 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 17:14:32 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 12 Oct 2022 17:14:33 GMT
USER ContainerUser
# Wed, 12 Oct 2022 17:14:34 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 12 Oct 2022 17:14:35 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 12 Oct 2022 17:15:18 GMT
COPY dir:4123bc4d354fb6abb19af459f2430680f89ba0d88861da6bacc3b060f799c08d in C:\mongodb 
# Wed, 12 Oct 2022 17:15:30 GMT
RUN mongod --version
# Wed, 12 Oct 2022 17:15:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Oct 2022 17:15:31 GMT
EXPOSE 27017
# Wed, 12 Oct 2022 17:15:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5ead999142ecce15e02523c49706a633fa708374d94bb65a254e3a3c117d609b`  
		Size: 103.4 MB (103377244 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3724c0f91ae729d3a2ed4ebab42f44a8e6cc1551989d86671030e217845bb6f0`  
		Last Modified: Wed, 12 Oct 2022 13:18:10 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da73564af28761834100addecae3d92a15038f15e90c074be483edb5c83adf`  
		Last Modified: Wed, 12 Oct 2022 17:46:46 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5866bd63b3c16f73b4117a6c07fd8c6a39d2293e69a833b08fb9980a34de3`  
		Last Modified: Wed, 12 Oct 2022 17:46:44 GMT  
		Size: 72.4 KB (72372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f0712d948b06cd11c6e8e73fe8bba98b44a8124b6b7308ec8e1bb8ae76415`  
		Last Modified: Wed, 12 Oct 2022 17:46:43 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a6efb0d0ceb84b3a98d28c5d5ff1356cf3fcbb1fd472dc31020c9065b8ca8d`  
		Last Modified: Wed, 12 Oct 2022 17:46:44 GMT  
		Size: 267.1 KB (267067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2596753edf5734fe3918ef21ea5e44cd692a72b8b0a6a4f8aea890ed34fe99`  
		Last Modified: Wed, 12 Oct 2022 17:46:43 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54662ca33fc7b874746038b71b12d444562833ae47079444f5b7988153646935`  
		Last Modified: Wed, 12 Oct 2022 17:47:59 GMT  
		Size: 511.4 MB (511354015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9763f8714ba38880a775752f35a613ee90043d23c34bb5c4a1e026df430cec25`  
		Last Modified: Wed, 12 Oct 2022 17:46:41 GMT  
		Size: 83.5 KB (83489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67dacfe89b2b263b56eaaa001785f0bc95f2885fb5cd0b4e40435aea204d43c`  
		Last Modified: Wed, 12 Oct 2022 17:46:41 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701acd4ebb164cedb232a803343b835c8c614ee66abef99afb17509d7805401c`  
		Last Modified: Wed, 12 Oct 2022 17:46:41 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99795f78afa1080832e29c18482fac3f1075ae4b1c8380eee67272d97a4ce85`  
		Last Modified: Wed, 12 Oct 2022 17:46:41 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
