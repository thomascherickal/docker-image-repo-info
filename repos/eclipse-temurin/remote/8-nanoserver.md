## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:72e8e74116e3706b90f30fb365e8e5940dcf7fd12202507c14bab6a85a2dd0db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.2159; amd64

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

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:80b359bcb4768b6ca86bf0e3235e58ea13aeaa61c37db16ab4fdd77ab85d0460
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.3 MB (206335402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:463ab2e03f4fac59d7a6b9a46f4f1a5218ba655ffcd19d19d9b9b0630232399f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:14:37 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:14:38 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Dec 2023 00:14:38 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:14:46 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:14:47 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:14:56 GMT
COPY dir:d9c44d909d2b41aad5bf6fa4f7c7d36e81063822ae5e7ef30e4851bbe7809503 in C:\openjdk-8 
# Wed, 13 Dec 2023 00:15:07 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bb2669772d53e8f301de1ada41d615e723affe44f15257b083be2409bd5db5`  
		Last Modified: Wed, 13 Dec 2023 06:35:07 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44b4904ea6c8d1f239630ac97b4c689e4a94e4c3f279c346157a468f5af1d0c`  
		Last Modified: Wed, 13 Dec 2023 06:35:07 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e9b3456b3ce55c0f25342c3ad8864049bee32fe4283c352ec02292102493e`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b0b8a38ceced0829a908f23f806d1767f63159b0a4a98036518e380d84fd1a`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 68.3 KB (68327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd4cbb70bf2ba8222fea4798880527b533dfeec77bccce2a922cd91dd128ad9`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd74c03ba177a5c5e9f1d3cd81e6cc648412ba3d79d5c0558e3ea2cf0e60994b`  
		Last Modified: Wed, 13 Dec 2023 06:35:16 GMT  
		Size: 101.7 MB (101670354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c249da5986f6e578ce93db0df5fdfb0f65f13eb7591611a5acc27cf1b3cb420`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 80.9 KB (80893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
