## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7067f36eba2d805bb62228484076e9344b3838d4447bba548f316f9dcecf22f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:fbbb58374a74699c92edea7b3e0196c272020f586c08cfe62bc2c24f37b1d74a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146904997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ee94d826f5959772c8064189ea563b8ebe6c10ad2d454e2a9b9da1cdb2f913`
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
# Wed, 26 Apr 2023 19:23:48 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 26 Apr 2023 19:23:58 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:5fc6409281dc9b2c9f9723f19374d9ff81a72dda326ad9ba6654b6db23bef41c`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 40.0 MB (39958239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988963f06d9cb6d35c9375486d98be5ee1823cdd672a758e4e48e938edda0508`  
		Last Modified: Wed, 26 Apr 2023 20:01:19 GMT  
		Size: 82.0 KB (81985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
