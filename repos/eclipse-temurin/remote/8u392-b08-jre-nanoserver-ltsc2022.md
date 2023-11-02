## `eclipse-temurin:8u392-b08-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:b46395953ddeff9b646b5f9b2d3d6462501fe7c7a7f98ff2174f0d8bb940d93b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:8u392-b08-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:24dfc0ae451adc97918ca1a43256d425a0a26b3c1a04c27d0b9d0a36e4e2ff1c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160861409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92c37e12a8b7485d233f1d4f2e6bdc3613b49278af80e21f847e3eae91d4790a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Thu, 02 Nov 2023 01:29:08 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Thu, 02 Nov 2023 01:29:09 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 02 Nov 2023 01:29:10 GMT
USER ContainerAdministrator
# Thu, 02 Nov 2023 01:29:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 02 Nov 2023 01:29:25 GMT
USER ContainerUser
# Thu, 02 Nov 2023 01:30:06 GMT
COPY dir:dbdf2dd9ed9894186d74b75beac1320724c73c6994b00118f04985f0ea2b3067 in C:\openjdk-8 
# Thu, 02 Nov 2023 01:30:17 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142fccf33f15e2c503ce4023e2e496d7a99bd036e8b83264772e9dab49c325b3`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca651b62b3002c026c9959a9e9fe771e9f5f6d921466075d9eac0843b844f3e`  
		Last Modified: Thu, 02 Nov 2023 01:35:46 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4dda019903db0644c71140f11e351633ccdb26fbbf27f1612511b147fdaf7`  
		Last Modified: Thu, 02 Nov 2023 01:35:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4a2f18b44a2dbbc87331b598fe2b697473f037035d8b202701a569d8a3e2c0`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262bb2d657e5cfc3b0ccaa6b40f822a41cf9e754f34778ccdb2c919fd1985ec3`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 78.2 KB (78246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ef65f0686e570e1a8ae625774530a802e34c839d058f642c0d39864485b93`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e379140e32b221fc75991ba6237948032d7d548f3150e02e142d74b35a24e87`  
		Last Modified: Thu, 02 Nov 2023 01:36:14 GMT  
		Size: 40.1 MB (40110942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2291a2fe8d713d98b997b03a26fc3ba0b5a690590e4f05821bc776164538a92`  
		Last Modified: Thu, 02 Nov 2023 01:36:08 GMT  
		Size: 62.1 KB (62071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
