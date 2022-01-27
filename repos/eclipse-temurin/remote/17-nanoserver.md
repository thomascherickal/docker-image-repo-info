## `eclipse-temurin:17-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:bb6aa0f81bea5387cb5575965b7268162890f39b6aa67b64922b038f2832b525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:17-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:546e2621d3b669fe25392c01915bbf06e5c4e60797adcc908b6fab4ec0a6a5e3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302436210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7825da623aba8bf0c21ad18a40bcf346ae1fd76f869056e26699b0782b88c4ed`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:43:57 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:43:58 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Jan 2022 19:43:59 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:44:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:44:14 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:44:45 GMT
COPY dir:75727e79a870c9066772bd3811959a8f3c491ac4b54ae3b2c145d1638b6bc93f in C:\openjdk-17 
# Wed, 26 Jan 2022 19:45:00 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jan 2022 19:45:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774536782c1c4d4015e8359ac0437fdb94a8d696f9cdef5e9936e721b99ae1f`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12214b1befa142979cea977dbe18e01fc824195c2dd83727fa5b15e41c38638c`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff8a2a945a4d41d4a21c3e74b99a007be23a149c47ec52f2f33ddf270bb6f16`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ada735cfb773a4d0ed93bd8768bcc1e11e8f13d0f5e8ebd60b41a1cb4c9f8`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 84.6 KB (84623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf9b071a062772e3a9bd393d34c0fae1dd2444a5298988e86b1daa21b0f785c`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b120bd4b75567bec8da9476b9a4fa54a253410cd5200f8f287ddb0b1ac941`  
		Last Modified: Wed, 26 Jan 2022 20:33:39 GMT  
		Size: 184.9 MB (184948777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21c3103dfa1badd3d0e807587ad95aa41ac5ea4fc2061f8d99cb18ecaf9c6a7`  
		Last Modified: Wed, 26 Jan 2022 20:30:02 GMT  
		Size: 62.7 KB (62725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc6eee220ed1f16365970800593bff5f2b404d5b2c7ffd5f08249675b972efd`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:c7898e105803c1ff00e51f3283bad7c6cdd1ca3fb31ab4a81578f74dc13ec6dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.7 MB (291717030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f9ea166b03f7dfcec309d6fa1fb2b89a104d50ae6f9af501c15369079d642ce`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:33:37 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:33:38 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Jan 2022 19:33:39 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:33:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:33:53 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:34:26 GMT
COPY dir:75727e79a870c9066772bd3811959a8f3c491ac4b54ae3b2c145d1638b6bc93f in C:\openjdk-17 
# Wed, 26 Jan 2022 19:34:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jan 2022 19:34:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159cc5ffca5107ce551dd80b9ed61ac450096630236c2247dc99f8d116f541c`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e919bba1969715a875c8d96965c2d78e044605cda42fcba99d9ab5f5a94e2976`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca96870c535b980f31c3d23beefcc204f3b3be6952024caa9e6b6a3caa8b8c`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2c81986540337ad2bf29c07de92b78dd583bfbb3a00a3e92bdd0714f9f8b29`  
		Last Modified: Wed, 26 Jan 2022 20:17:20 GMT  
		Size: 68.0 KB (68032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b57584fe1a0c2ff5aa5a8ed4aafa3786359488ae67aff438b6fa1e4e3cf31f`  
		Last Modified: Wed, 26 Jan 2022 20:17:20 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1520ae93a3f16aa928da757f288f9b4d94cc7f06544054130f1feb7ce8f6a6c6`  
		Last Modified: Wed, 26 Jan 2022 20:21:01 GMT  
		Size: 185.0 MB (184950496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9288b72d40d6ef64d3406bba8b5308787a981b990964e8b7b6b758ca46ceb80`  
		Last Modified: Wed, 26 Jan 2022 20:17:21 GMT  
		Size: 3.6 MB (3645038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d89a9a0d3444a86fe189fce6abec8cad2a0e18b49267a60f25d5ee93722be`  
		Last Modified: Wed, 26 Jan 2022 20:17:19 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
