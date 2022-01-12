## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:948e359014041ea1a4b7edde16d52f2eb5de30adbec0e9d09cc31d50e5551e6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:45b7bc29e3764b3fc689a2b8cde59f10c7931618f4ab5e362839019af51e842d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203373307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5fe0c9ba09af56a271af90058a25ba2c1b400f1561606ce5734ef2d1d4a38f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 05:19:56 GMT
SHELL [cmd /s /c]
# Wed, 12 Jan 2022 15:34:02 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 12 Jan 2022 15:34:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Jan 2022 15:34:04 GMT
USER ContainerAdministrator
# Wed, 12 Jan 2022 15:34:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 12 Jan 2022 15:34:19 GMT
USER ContainerUser
# Wed, 12 Jan 2022 15:34:37 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 12 Jan 2022 15:34:50 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:71dcb756adb8534a87210067788d6aa4a5a366b72d022b7af035e5263a3e54a0`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9688a822af3207c76f479e1dcd24729a872b14ca7b578a5cf939c8da1beea82f`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9392e95e3451d5255c7eb6f7082ecb82e722cc977e6a4e482dd4f191928d78e2`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff7ad2a002508b7608d2069eb80fd73536913d79f8a080b2306aaac7967151f`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d3d451d5b86383a9c3ed5b112c411d530439c1306c852d24920a9e3cc74144`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 69.0 KB (68977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3aacb454a880cd5cf940cca71b6570e6eabd1e99834bba212fef2aab817436`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25335eb984553f45fe31b623d29beed47507e001b21742a1ca35d8740ed03ab7`  
		Last Modified: Wed, 12 Jan 2022 16:05:27 GMT  
		Size: 100.2 MB (100186381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5121097c352d366839b63ee98e87cf4c1198effdd73c5d1b5fecacb3ea5526bf`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 81.1 KB (81073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
