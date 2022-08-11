## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:938181b67d0fc9cf110dc0a49efcd2fbea92c58b262bff6bd9d48dc1cb6d7770
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:0510f95aefaa0428b5a67d837d4da87ef5c992b5cd6de414668a66afabd9c7de
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157557594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4dda98cb5af421df59895bf05800917071851a69344d44eb8b8da119c84b7ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 16:28:17 GMT
SHELL [cmd /s /c]
# Thu, 11 Aug 2022 19:27:02 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:27:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 11 Aug 2022 19:27:03 GMT
USER ContainerAdministrator
# Thu, 11 Aug 2022 19:27:17 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 11 Aug 2022 19:27:18 GMT
USER ContainerUser
# Thu, 11 Aug 2022 19:27:58 GMT
COPY dir:8b6137b055df5a3c6f914a172c41a8287046696fe7ccc91d96608246e3752adc in C:\openjdk-8 
# Thu, 11 Aug 2022 19:28:10 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f1e06146ab0490d235fe89786637467a4b71853ee428e8740ea6efbc536c47c`  
		Last Modified: Wed, 10 Aug 2022 16:48:40 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770dc366b2a629dc8c50641df646370966b4a3b3af562ea794b426e47acf9c31`  
		Last Modified: Thu, 11 Aug 2022 19:33:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b30283938410a8d67cf093632a7d78906fb7b27cfea2ff00306bdc483cd6c6a`  
		Last Modified: Thu, 11 Aug 2022 19:33:43 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46b60d96d227e29a4c5423868410757fca4a805b6f1580031c016ce5aced9`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2900ae6f8b3a3c35c67bab56131b7dd5a1e658998d1a2002244f6783d06019d`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 84.4 KB (84440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54070f1ff08a7ab0078fc469730bb289ce25ea935871b8c6d4447f590ba639e2`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e29fd40fdb52c086ffeca260f9e2e16dee1c44f64218b2e836086068ec2f99c`  
		Last Modified: Thu, 11 Aug 2022 19:34:10 GMT  
		Size: 39.3 MB (39317029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff26e42dd2219ad2f4d0be869c16d82d799f72f41ee92eeb21293ad7032b61e7`  
		Last Modified: Thu, 11 Aug 2022 19:34:04 GMT  
		Size: 61.9 KB (61912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.3287; amd64

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
