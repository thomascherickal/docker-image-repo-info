## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:fc5246682ab0695c8bad69f910289cb894a1076b8bf7f47fedc4b4712ae1eb75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:ded1952642431a1d3ffd4b133733de0449268eee450a7a0369c5ed6a5760e183
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.1 MB (203065449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c15a93b2bb46b6171a4963a9d95acd8ec97f598dd77519cd7af30c244980574`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 16:34:08 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Wed, 25 Aug 2021 16:34:09 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 25 Aug 2021 16:34:10 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 16:34:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%         && setx /M PATH %JAVA_HOME%\bin;%PATH%         && echo Complete.
# Wed, 25 Aug 2021 16:34:25 GMT
USER ContainerUser
# Wed, 25 Aug 2021 16:34:36 GMT
COPY dir:6622177b1379d4d7267ebc9bc4d0bb013ea883bae36028c72b4045f7fa088598 in C:\openjdk-8 
# Wed, 25 Aug 2021 16:34:50 GMT
RUN echo Verifying install ...     && echo   javac -version && javac -version     && echo   java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c67b6d91c42638469dc7118f17ff6144b76a58808c348c7bd2b9f2396c7d6cc`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a828ecaca576c5ae13538f466aa044a6196d1cc9351c3bc0edbca0a64110d621`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9b5820d1a79bfade7332d3b9792fe0de92dca4316f12e566a0b23838e1001c`  
		Last Modified: Wed, 25 Aug 2021 23:21:11 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5244bf4f583093a25d20693bd5e9041c538db73a9e1ddd118fb7f3553d198`  
		Last Modified: Wed, 25 Aug 2021 23:21:12 GMT  
		Size: 69.8 KB (69803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7948b5ba02199260c73e70bb471b3a443ccf0406a189981c41e3a732a1741f`  
		Last Modified: Wed, 25 Aug 2021 23:21:11 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5932d5d4ce162aa5027cf5459c722437263db5c63f0a3141aa17a36dc19968`  
		Last Modified: Wed, 25 Aug 2021 23:22:55 GMT  
		Size: 100.2 MB (100158395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a28c7b58cc61ca17d6b131106d7aeb315a6fd91d18d2f54af526e5e8acc647`  
		Last Modified: Wed, 25 Aug 2021 23:21:11 GMT  
		Size: 90.8 KB (90837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
