## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:9fe4172c308fda8822c86d803f3caabf8b7e3e4956d6e7702159a0241e4d6276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:33979c8132ddd177cebde8cdaa1c50b283e93fb270c61da05d71a1c0e2d8360f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.0 MB (147957695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e8f2f303ad4fc9af31e911601fca6184693429b408a07ca716193d78c410993`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:19:54 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:19:54 GMT
ENV JAVA_HOME=C:\openjdk-11
# Mon, 30 Oct 2023 23:19:55 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:20:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:20:06 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:24:12 GMT
COPY dir:32725fa0f7edeee10e8937816f70b588636369ca6a0eb68560cc5c3b2b3f76d9 in C:\openjdk-11 
# Mon, 30 Oct 2023 23:24:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40516a6c795a5f06ec243811551b8495a45915b7ba984b8141c7523b5aa7f2bb`  
		Last Modified: Mon, 30 Oct 2023 23:48:55 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022e2c9d36c484c8ee07c5ecdc37a4c33d28b4a02e81ece918a256ffe4cbe72`  
		Last Modified: Mon, 30 Oct 2023 23:48:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4183a8bbb10b3dbbd7255535286443c32d3166050544f0c78522cb8b9f59c24`  
		Last Modified: Mon, 30 Oct 2023 23:48:55 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06da08f655ecbb3448f861b2c91ca77a812899866a43471a9514742a19154e9e`  
		Last Modified: Mon, 30 Oct 2023 23:48:54 GMT  
		Size: 67.9 KB (67888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9341310d47d0b19efa76ce536a673583cecb7e355832c7c03c4fc579554b546b`  
		Last Modified: Mon, 30 Oct 2023 23:48:53 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677d5ef4bbf305aa8ce2da344f1781933813140daf45341d1218223fe0fe0c3`  
		Last Modified: Mon, 30 Oct 2023 23:50:05 GMT  
		Size: 43.3 MB (43339695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b3f565b3458e50b6ddcf61f0beb3b20bdf606d977736cf60e0ebf471c76bc1`  
		Last Modified: Mon, 30 Oct 2023 23:49:58 GMT  
		Size: 79.9 KB (79861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
