## `openjdk:20-ea-nanoserver`

```console
$ docker pull openjdk@sha256:fe91d700ac37564640d2c09c5a71f9fdda3fa065bdb3a2a444dd72bf6cfc546e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `openjdk:20-ea-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull openjdk@sha256:f062c80bd52e570278be7c050010789e4be0c40388b3c2523e7596ab66be8da3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.6 MB (303623107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2e2d6bec9c0ac0052ae8cbda1b9b3dbce043daa2c894f6f7c6b12d2d930ece`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:45:31 GMT
SHELL [cmd /s /c]
# Thu, 12 Jan 2023 05:15:32 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 12 Jan 2023 05:15:33 GMT
USER ContainerAdministrator
# Thu, 12 Jan 2023 05:15:42 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 12 Jan 2023 05:15:43 GMT
USER ContainerUser
# Thu, 02 Feb 2023 23:30:19 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 02 Feb 2023 23:30:36 GMT
COPY dir:987afce70a813d739c5f0b86f5b3b61438b3da1248b0a1ad2aae21a46628640d in C:\openjdk-20 
# Thu, 02 Feb 2023 23:31:06 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 02 Feb 2023 23:31:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea67a6bd980bdee35399883e5abcc31c738b338ad384b2f92d91a15cf09d9df`  
		Last Modified: Thu, 12 Jan 2023 02:40:16 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96518e54215f38193b505640cdb2fef097c5741e65b4b97bba8f867e243d032`  
		Last Modified: Thu, 12 Jan 2023 05:25:44 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63c92ba435f57ba529ea551f43866f6d4eba3a81d296b0fb044c740f2ee807`  
		Last Modified: Thu, 12 Jan 2023 05:25:44 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b356ba1f31bf25142c630cbcb07b081461c3f630e690d98dc24ae4786a9ef7a`  
		Last Modified: Thu, 12 Jan 2023 05:25:44 GMT  
		Size: 70.5 KB (70518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638383fe215678a48f17d26ca2a40f4c79f0e0929d53790d7d9d5d1d73cdb9cb`  
		Last Modified: Thu, 12 Jan 2023 05:25:42 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc2e86a14155069a7f64814bdee7c899cdcea478583b9ef2cfd4e1b4dc1796f`  
		Last Modified: Fri, 03 Feb 2023 00:27:05 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a315885cade1f83d92ec89e7763968ae165f7d8cf14714985a8fbd38cb1379`  
		Last Modified: Fri, 03 Feb 2023 00:27:28 GMT  
		Size: 193.1 MB (193081466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3abec91f61f1a422000043000463b80f01e4504db4e3fa6c6148e58423be6b`  
		Last Modified: Fri, 03 Feb 2023 00:27:06 GMT  
		Size: 3.8 MB (3798245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd075197b7ef9cff6f7e60d5fb5785db7b73f2272845c346cd7dadaa7817ef40`  
		Last Modified: Fri, 03 Feb 2023 00:27:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
