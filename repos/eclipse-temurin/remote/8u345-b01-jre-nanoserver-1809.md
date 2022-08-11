## `eclipse-temurin:8u345-b01-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:1b17ae481e3d91ba0cac95bb9eefc92f061c2f271efdce5d8b653bcee7111305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8u345-b01-jre-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:ce61f3adf4d6882784c5d0cc9e068469d2bb483b17d47657110c13169eb334a8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142682947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44432f727522d2836c7e4988b64e2b076e0e2c5b2a2a927000d927cc1facd342`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Thu, 11 Aug 2022 19:20:23 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:20:23 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 11 Aug 2022 19:20:24 GMT
USER ContainerAdministrator
# Thu, 11 Aug 2022 19:20:38 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 11 Aug 2022 19:20:38 GMT
USER ContainerUser
# Thu, 11 Aug 2022 19:25:02 GMT
COPY dir:8b6137b055df5a3c6f914a172c41a8287046696fe7ccc91d96608246e3752adc in C:\openjdk-8 
# Thu, 11 Aug 2022 19:25:13 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fd3474e767c89d4884899365be25930e54c53f51a074e69cc02802725ae6d5`  
		Last Modified: Thu, 11 Aug 2022 19:32:12 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7647596c60b4a6ad1f5ca775c5fd3f55ff77837639afff14c18ba7835f2308`  
		Last Modified: Thu, 11 Aug 2022 19:32:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41014c3c1e1598b5823b5cfb25e91bc92911535419ec9cfacd6999e6d75c287d`  
		Last Modified: Thu, 11 Aug 2022 19:32:09 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a389d300354d5cae214dd02ea0250b75df400fc6dbdfe3a86010e1f0d8c3adbb`  
		Last Modified: Thu, 11 Aug 2022 19:32:10 GMT  
		Size: 70.4 KB (70417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc85db5fff9936a95dff8f64641330a3b012a5f63626ce212e03a832c9e2aed8`  
		Last Modified: Thu, 11 Aug 2022 19:32:10 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61814166d0deee00656fe7f35bec36664e5df7157c613949421d7d3fe7cebf59`  
		Last Modified: Thu, 11 Aug 2022 19:33:15 GMT  
		Size: 39.3 MB (39320930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b4a7dbc132c54fa81fadecbc1ae8d30bbb6c1cf4cf9b155d23498a95c61f9b`  
		Last Modified: Thu, 11 Aug 2022 19:33:10 GMT  
		Size: 81.6 KB (81588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
