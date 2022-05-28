## `openjdk:19-nanoserver-1809`

```console
$ docker pull openjdk@sha256:754090ddd7aab4ccd51c96a5d68679ad122dc698678c1f12860b297ad6bb39e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:19-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:ac8eff8869b25be38adbe801e4dd1c1c3c72ee712cbb4f955636cc523a6d8a42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297523551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2fdd94015cf33431caa640bbc810779e87e39539d54c1015699b33437739de`
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
# Sat, 28 May 2022 01:18:32 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 01:18:48 GMT
COPY dir:57cc2db1e2b982614a7138a4dfb149c4cdc1a1e9f94dfcc86a255d8507734b7c in C:\openjdk-19 
# Sat, 28 May 2022 01:19:10 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 28 May 2022 01:19:11 GMT
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
	-	`sha256:9f5a9b01b1cd0da119db574745cfe5c5a2702e86e23326d3e7e85b3e8e2ab8c5`  
		Last Modified: Sat, 28 May 2022 01:25:02 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124387cd4c7e842eb4bd4b97fdc38d8825e1eca38aad92cbf7d6e31003dc7108`  
		Last Modified: Sat, 28 May 2022 01:28:18 GMT  
		Size: 190.7 MB (190663291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996569f4ce8057421b012e10f1b8510528320ce4893d4d5528a37a6edbd88132`  
		Last Modified: Sat, 28 May 2022 01:25:03 GMT  
		Size: 3.6 MB (3644980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c2cd14b1e60e9a88b6c760feea8fe4c33ae11c32f78ef5968538f7c89fda6f`  
		Last Modified: Sat, 28 May 2022 01:25:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
