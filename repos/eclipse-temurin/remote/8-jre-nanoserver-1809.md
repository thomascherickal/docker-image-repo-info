## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:45551b6d8992f79eb29f4469af8c634cbc9cb5e8ecf5e84fe6aa32b557bb6263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:bb8d73b704731bd1be3914ba2f5e258c4f84c9f867cf9c6921b77ce399132ca1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144506285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87138bfa119bcf779d3693c2eab4bc3d07fd501678b8ea1d823b38e75b83d46d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 17:41:43 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 17:41:44 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 14 Jun 2023 17:41:44 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 17:41:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 17:41:57 GMT
USER ContainerUser
# Wed, 14 Jun 2023 17:45:13 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 14 Jun 2023 17:45:25 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db019f0eac9dcad0cfd76829e0606fc3759641cb53511bb3535cef61aef4fdcf`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272fe80b4ef0ac5c142d767c7636d470570914eb09cafa7acb9984b6f8ab29`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924439698c6ac9e1f4c8e162caf6843a1755893cab4179758aa40c021db2586d`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d176e42bd3de2c765eda8b596b2ef0cf0a6fc0aa32de0848478174ef196d8`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 69.4 KB (69404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5302d03e13870dffbd24757833957ab84dbeda5c04da418c30766476648b1bee`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d7fc070d91c16da80821ce07b0e7e904a87713689bebf37c45483262a6be61`  
		Last Modified: Wed, 14 Jun 2023 18:27:59 GMT  
		Size: 40.0 MB (39952230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10599090b2480c2c42f0beacb0188fd16df6bf6ca82b9f8bf097a67882be3a7d`  
		Last Modified: Wed, 14 Jun 2023 18:27:53 GMT  
		Size: 81.0 KB (80955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
