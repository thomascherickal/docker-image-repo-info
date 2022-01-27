## `eclipse-temurin:17-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:3af50b3fa226048e45731f11d3e1d745233c17155f6135465de977a908ca26c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:17-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.473; amd64

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
