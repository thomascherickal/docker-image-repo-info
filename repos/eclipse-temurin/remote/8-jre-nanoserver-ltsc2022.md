## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8b1402e63f0f3927a46fbada511d6e2986b4a808685eaeb1f883e3b41e873c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.887; amd64

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
