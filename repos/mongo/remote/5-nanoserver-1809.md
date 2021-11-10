## `mongo:5-nanoserver-1809`

```console
$ docker pull mongo@sha256:3c06c59945ca6e90695b0a06af5dad679d87f63d0dfec25e72447160db4d4a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `mongo:5-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull mongo@sha256:5ecb4d1a437de841dea302abfd45c27a8d4190363cd5aa09118ccb38cc472852
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.3 MB (395302826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09aa1b5f4f58f392393dd8725c3be30a0d3638c3d820d52f50dc630bf626e8d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 13:41:43 GMT
SHELL [cmd /S /C]
# Wed, 10 Nov 2021 19:14:13 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 19:14:28 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 10 Nov 2021 19:14:29 GMT
USER ContainerUser
# Wed, 10 Nov 2021 19:14:30 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Wed, 10 Nov 2021 19:14:31 GMT
ENV MONGO_VERSION=5.0.3
# Wed, 10 Nov 2021 19:15:01 GMT
COPY dir:baac5d5282a412454e91eae7dd7233043d96306f42a1848f6024087e0035bcb7 in C:\mongodb 
# Wed, 10 Nov 2021 19:15:13 GMT
RUN mongo --version && mongod --version
# Wed, 10 Nov 2021 19:15:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Nov 2021 19:15:15 GMT
EXPOSE 27017
# Wed, 10 Nov 2021 19:15:15 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9fe7a02124d29cd21b5f6d5ea22a1ba3de09099c347d1d0c0e2d89e650ddee00`  
		Last Modified: Wed, 10 Nov 2021 14:07:31 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a0459f3f99e74f05a8457e55c1f306a65f91eb620f2b335f36b49ce70f8d2f`  
		Last Modified: Wed, 10 Nov 2021 19:40:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90c3faaf1ec3abe7f2c84c50d3e74483cba21bd14918c5273cd7577764bf12c`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 72.1 KB (72092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b354c743ddd6e6dab3fde4cc72bf3fbf21fd4f2f69d57bdb71b204ddbe92c5`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81adde81af5d22a9d13bbc929d2143462e050a3c821a78a755b210b322b993`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 274.1 KB (274065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ce93f48a937d53ceb6b861bc41c63e61106ce53008ed97c2fed3c3f3165913`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552a462a70b984b58d9764855cd47ca5248021f7b1dde074c137403dcb58e590`  
		Last Modified: Wed, 10 Nov 2021 19:46:08 GMT  
		Size: 292.1 MB (292116446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47982121b0cad4ec74dea81f2740e63e5475c6ffd592629f10bcfa060e6b83cb`  
		Last Modified: Wed, 10 Nov 2021 19:40:55 GMT  
		Size: 49.2 KB (49214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dc5226e6ca87a13b8466dc66ac4d953a6f86d78fcd9c7955255d198aa1eff2`  
		Last Modified: Wed, 10 Nov 2021 19:40:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c465eb74d537679c31bc2970f570191ae0b744890ab7b4fc4f2b735e88763254`  
		Last Modified: Wed, 10 Nov 2021 19:40:55 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ce8be1091479a3edcab4bdf2ed0b96bbd81bb35b31b84c73a62e895bdca9b5`  
		Last Modified: Wed, 10 Nov 2021 19:40:55 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
