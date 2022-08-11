## `eclipse-temurin:8u345-b01-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:802376f1e196f49bdca22cdf168b983c9cc9244b540b62108558695cfc7356ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `eclipse-temurin:8u345-b01-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:ab4cf65c380a478baedc31f1ef10e4bfce01e71b635817b5a79f91b3bcb61381
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218710837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ecbff83ea28867efa129a69cf315409c66d37dda905555d242ae0539d00405`
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
# Thu, 11 Aug 2022 19:27:28 GMT
COPY dir:3f2d3aa63ba7a56176deaae1ba1b26dbdbe105074828954c77b0da527aacd6d7 in C:\openjdk-8 
# Thu, 11 Aug 2022 19:27:46 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:523f8d7b38db71243e121938cb6f33d7520bf0b80f4d61c2fb5055b8fc398da9`  
		Last Modified: Thu, 11 Aug 2022 19:33:52 GMT  
		Size: 100.5 MB (100469425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258123d28cc3c8a7f57c9ef7629b223faeeacc72795ef2cf1cdfd378ea4fee3`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 62.8 KB (62759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
