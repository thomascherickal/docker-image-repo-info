## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:e482f16484e7139f0ca281d8fc1574a5f30aa170f0ba961aee8c251114cdd55b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull eclipse-temurin@sha256:9b37953dd021fd2d09c28db7026f87396eeb1dc5de6cbc184cf3468f7cec3d40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206021238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f65b9ca9d34d9568123b812242133aad0d5334a48e24985cfa42932a465bb25`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Tue, 01 Aug 2023 21:19:45 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 01 Aug 2023 21:19:46 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Aug 2023 21:19:47 GMT
USER ContainerAdministrator
# Tue, 01 Aug 2023 21:19:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Aug 2023 21:19:57 GMT
USER ContainerUser
# Tue, 01 Aug 2023 21:20:09 GMT
COPY dir:809f08e9d949f52aad6441d5338932efbf6208a06192d58db41d3e3c11ba3f9f in C:\openjdk-8 
# Tue, 01 Aug 2023 21:20:20 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c8394d64f526dec4ca3b20eded3b04f3a527669ee1d94b1c3a10eb76c7c0f3`  
		Last Modified: Tue, 01 Aug 2023 21:31:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dab1f3820ee6e69eb56c90cb7b89474eb05e0c7373793a3b755cf008f36b85`  
		Last Modified: Tue, 01 Aug 2023 21:31:19 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7135c46d9193a51c931c7c64e294600786a8c378ba679d14808f41e4c512fc7`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d61f4df5c7e0aa60343496495b61390672968a9b62b6683a9321df9f99b4317`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 72.6 KB (72611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1739e988680aa09378fe65cb99374b0be5bfff70eef733bc756693f5546cd96`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1a043c59395407073ae87c27cd067cf0324cc7c6b47b5f66ecf0223ecc52a3`  
		Last Modified: Tue, 01 Aug 2023 21:31:29 GMT  
		Size: 101.5 MB (101484104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cf18a3f4089efaf18029b9ee571f4c4da20d91870c966693382f32ddd5cbfe`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 50.5 KB (50517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
