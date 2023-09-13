## `openjdk:22-ea-14-nanoserver-1809`

```console
$ docker pull openjdk@sha256:0d35c26d306ba495d231cdda534b9c44ac216f80af294acf6fd6b4190bffc55c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `openjdk:22-ea-14-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull openjdk@sha256:3f4d40a052087ba3d1154edeaec2ee65526b2d2b175ab3ab5568d92c9dfedbd3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.4 MB (307374325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67000b07ca22e072b88c8f8035f5300d0ca2dea49bb66793b42455498fab493`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 02:29:44 GMT
SHELL [cmd /s /c]
# Wed, 13 Sep 2023 05:19:19 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Sep 2023 05:19:19 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 05:19:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Sep 2023 05:19:25 GMT
USER ContainerUser
# Wed, 13 Sep 2023 05:19:26 GMT
ENV JAVA_VERSION=22-ea+14
# Wed, 13 Sep 2023 05:19:40 GMT
COPY dir:3e93a63762464c4297fd9a428ab7cbf0f98d649f815f43061cc035465db3383d in C:\openjdk-22 
# Wed, 13 Sep 2023 05:19:48 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 13 Sep 2023 05:19:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a5bcbc9b0f0398bf8f14c235b24ba85d9acacf855518119cd1ce338a235a15`  
		Last Modified: Wed, 13 Sep 2023 03:36:33 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6f344751fdeca77c774720f1f5845e2a683d1ed1b251bd6e554f91ab03d2b0`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be8c52d7c546ce325f7f3606c55b22e94fd1925aba26440028f33d2a873ff1`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de794e4f653951d19d788489e6c197cbbaa2864a36a169d068b25cf13ea0c6a6`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 79.5 KB (79476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4673df9416ca713de65ecb18e35ecfcad8bafedd6b1e61dca148de841d138b7`  
		Last Modified: Wed, 13 Sep 2023 05:26:44 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8ea94378b2c030d13122d77d129b17ae8b43d2e9ebbad87d40b9225b6f83b1`  
		Last Modified: Wed, 13 Sep 2023 05:26:44 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d175eeb164beeed060a832ca70d255b5d226c9da179a7ad45cf209783189b18b`  
		Last Modified: Wed, 13 Sep 2023 05:27:04 GMT  
		Size: 199.0 MB (198988318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f60722dae3bb96c709310d835cfac35b6f0e451cf2984fdee3566304ac4eb89`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 3.8 MB (3807044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6e40dfc5c1fd0a74b78951c77cee5ee87a42d811e45316bff913e729bad837`  
		Last Modified: Wed, 13 Sep 2023 05:26:44 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
