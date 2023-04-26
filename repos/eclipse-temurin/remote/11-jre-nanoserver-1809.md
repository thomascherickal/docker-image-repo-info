## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:a0451748db4bae21b3758f4da88ad0609fb417a11d036565942dd6fcc6d3d21b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:9c5fbfc7bd0aa58155bd0cb5ba2eefbe82f85f4770feec588e0b8adc811fb790
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150112870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e072a4f5646639bd298476144c1d29e959d8c5d9c5d2c73557e30aa1147a6b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:28:44 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:28:45 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Apr 2023 19:28:45 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:28:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:28:54 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:33:18 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Wed, 26 Apr 2023 19:33:29 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce4e3b8bac3b5d03c157f45ff3320441042109d47d3c0da2bc3a194fe9ad5d2`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcefac68112b666cf61ad6362f369d8237f25f4ee5909e378f8a13fcc4c9fa7`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1cad6c030895845be45eeba53c24091757fc1b01db3496ab4752ba176033a6`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714f5674d7b5a34fb8f58301a6da94389dc78a251455c2187934ec36d475bbc5`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 68.5 KB (68504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66362b7ce52315d1faed7636cd5df8b075c26119726a777008f0c74958639b8`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8305016bf437fc7e2f5f7223fbe8ca513db0f936f2b698a4464f18b4ffd805ec`  
		Last Modified: Wed, 26 Apr 2023 20:04:03 GMT  
		Size: 43.2 MB (43172600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997951efbddf203103baad5448b850ea8e47019f2333b8e3b426114faa0dbc58`  
		Last Modified: Wed, 26 Apr 2023 20:03:55 GMT  
		Size: 77.1 KB (77079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
