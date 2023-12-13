## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:63b7b510411e9eaae0d663a17e502a81d06b2c0fbd440ec5e30a986a823b1912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:5a80dd596b7a4715370f788c14576e505042b2d74e1bfa4aef6c94a258ded55a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222598492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38073e743105674ee115fa39e0c417641935d3f7616688c64cd13da98a326de`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Dec 2023 00:49:14 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:49:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:49:43 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:49:53 GMT
COPY dir:d9c44d909d2b41aad5bf6fa4f7c7d36e81063822ae5e7ef30e4851bbe7809503 in C:\openjdk-8 
# Wed, 13 Dec 2023 00:50:07 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420e231f6e0404269e9ff487f0ffc079de3deb8c08e9ff31ccb5fda1d1a44ec`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf164bbdfb6f48a324b0a202412c204a0fe367efe5829ef14105bbd65605b66`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e516ed43c06e2b90a2550de28ed9e594a346fd4668e2807446ad69e0744fcd74`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf7cc4c908cb1abf6fe51888bc260f997343bd25220752f0d3b86076713ae1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002dbdb57bb357c987be5ff6bcbc5e3cd108805d231b7f09809337c5f36e2ba1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 85.5 KB (85519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2219f416115f1fbad27502353948edc25fab0d18bd677b2b058840104dbdc94d`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b94f2b665f78dac1836bfb740543ebb7228439e1391a1ca5f15fc580a1a4e4`  
		Last Modified: Wed, 13 Dec 2023 06:44:27 GMT  
		Size: 101.7 MB (101688066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb7e41d0d916ebd63cc5269829560dbbd6c50dfd6f8d3480379ff8260039dd0`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 62.1 KB (62081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
