## `eclipse-temurin:8u372-b07-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:80c73ea032f3d82fd4c6d1f5d0800b31a9a899261e34c537f18a1e714cc1b3a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:8u372-b07-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:c3c2d3dee46f2932aaaf20482f4ae8fceaea6f00612024883e834b37f5de953e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208391816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c3a485944fb7b3a3e875e3b78958550abc98a1d6f5c1763f7def645e6d3aff`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:19:33 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 26 Apr 2023 19:19:34 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 26 Apr 2023 19:19:35 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:19:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:19:44 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:19:54 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 26 Apr 2023 19:20:05 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3503828cf095dded0c0d7dda78c9be78ae11cfb3204f872487d7b7af137291e2`  
		Last Modified: Wed, 26 Apr 2023 20:00:25 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a858798fd8ea05fb2a7b8d691c142d00f297018fc3a052125124f1f44dd1cf2`  
		Last Modified: Wed, 26 Apr 2023 20:00:25 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cda215bb64ed53246d0b0f22122854bc379a5ce2ed03ad65ae99c2b2af62df`  
		Last Modified: Wed, 26 Apr 2023 20:00:23 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24be090e79065dfd710fa2b4ad22e6adbec0ea5d77a0469f9fbd9c3c08bacc74`  
		Last Modified: Wed, 26 Apr 2023 20:00:23 GMT  
		Size: 70.4 KB (70371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14e2139efd02e67fe37c62d541a0217610314c913cb228960ec4dc3234a6a4`  
		Last Modified: Wed, 26 Apr 2023 20:00:23 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77a4ce8f5f92e037514d5e77c4084156e557b6ec973ac2fdc1e057763913d38`  
		Last Modified: Wed, 26 Apr 2023 20:00:33 GMT  
		Size: 101.4 MB (101444320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8de47448099ee9d619e5eb3d98a35e37b1a8f3b26483fb5e0209610e2463dcb`  
		Last Modified: Wed, 26 Apr 2023 20:00:23 GMT  
		Size: 82.7 KB (82723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
