## `eclipse-temurin:8-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:14834061694c69306aac2c41be7a36657621fd59bde8cefb1c2847f540301b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:8-jdk-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:f5b4b0bd31ddcea2bbeda777786dc4384466e958b74a01e7ae6974cbb2cc23f5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.1 MB (203070294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff9d22c48aa42b788c02cc39828d451e1ffbdfbd1890487c9e1edf991af46689`
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
# Mon, 13 Sep 2021 18:19:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 13 Sep 2021 18:19:11 GMT
USER ContainerUser
# Mon, 13 Sep 2021 18:19:21 GMT
COPY dir:6622177b1379d4d7267ebc9bc4d0bb013ea883bae36028c72b4045f7fa088598 in C:\openjdk-8 
# Mon, 13 Sep 2021 18:19:38 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:157ce3ea050d2a275c206be8e1c13112a5dfc8c9e966189d63ce0aba80055340`  
		Last Modified: Mon, 13 Sep 2021 18:41:48 GMT  
		Size: 68.3 KB (68251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adc073dbdca97ec186ebfa597ad843e737d0e5ce32901f4ce12ad769c43968c`  
		Last Modified: Mon, 13 Sep 2021 18:41:48 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4926858dd57408abaaf1a222db025d750fd6a00cbd338d225fea391ddb5b10f`  
		Last Modified: Mon, 13 Sep 2021 18:42:00 GMT  
		Size: 100.2 MB (100166173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b901fb7372db014775aac6e428b4d573a382b67511c17140651316a81460c071`  
		Last Modified: Mon, 13 Sep 2021 18:41:48 GMT  
		Size: 89.3 KB (89311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
