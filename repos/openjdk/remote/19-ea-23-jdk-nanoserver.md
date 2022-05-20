## `openjdk:19-ea-23-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:8578bdaf2233dfa1eb6c4da33e6dbcce8ce4f7a4db6883e90272d4283c8be54a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:19-ea-23-jdk-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:c76970c9c1e9d42f4bdc91d3a48a79342047ea7e0c1e29c275993cf836b931a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297475193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb90e79750e6883274732dcdb1c5e703c67195df5628e76619f92d52e68c687`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:33:35 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:33:36 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:33:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:33:48 GMT
USER ContainerUser
# Fri, 20 May 2022 21:18:49 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:19:04 GMT
COPY dir:bb866da67e95e37851148d95ce6f74d09a073d10afc6a53184a3ff0098abc9d9 in C:\openjdk-19 
# Fri, 20 May 2022 21:19:28 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 20 May 2022 21:19:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27258317e27e0cfabcf779836e0e38e0809f5ba5b2e2ce61b0c4761494eabf2f`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f575ce9dbc595a6266a2d907de169473af97a71414d6a81d122bfc9cd5e39`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40175500d750084c8212d8ea8f70d757ec3255fcb2fe588e2663c8a405187094`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 74.5 KB (74495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d665e0106401630d154ad3a944dc128966740b1e1b21d2fbeab345b8da177a`  
		Last Modified: Wed, 11 May 2022 16:00:31 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a73865feacceb513e5677af344491f5593efdfe1ae28003e4cbc042dc81a`  
		Last Modified: Fri, 20 May 2022 21:28:34 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed86c0b7803b2bb83b467fe79737dace8acc7de9c911cb1a846e5623ca3e88`  
		Last Modified: Fri, 20 May 2022 21:32:01 GMT  
		Size: 190.6 MB (190613986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92be9991aa4b37a47769bc1ff2234603109c6a179c2d0b4bea987115733a6c69`  
		Last Modified: Fri, 20 May 2022 21:28:35 GMT  
		Size: 3.6 MB (3645951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd50ff5886fc6a06a42ae369b78e288e107e1cf57be447b2dc7c16c4616e71c`  
		Last Modified: Fri, 20 May 2022 21:28:34 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
