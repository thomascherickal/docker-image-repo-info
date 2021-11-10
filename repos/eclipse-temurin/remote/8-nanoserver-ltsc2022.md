## `eclipse-temurin:8-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:a7992340811016c06704f596f5882c9b2eb250acb55426c0d38fd5354106b27b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `eclipse-temurin:8-nanoserver-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:bca3801c0736a4cf5823f428170088083c9764db5066d3c7b312321150fd4731
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217482274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a2a5f5a4c5b0c9f9f0df086acae7a3ca1431a49626374b545644d8e41303e5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:52:20 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:52:21 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Nov 2021 17:52:22 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:52:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:52:36 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:52:46 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:52:59 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ceb9b6cf720f75473e3c41307d287700ff9e2fcbb1e7fd036ed7a78a6c64e4`  
		Last Modified: Wed, 10 Nov 2021 18:53:57 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61655ff5d6ffb4e9b28c5bb62ef4e6838797460f0b1136f043b2cd0599eb5190`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f8ab0cd19e99cc99b76ace65f501d956fbb5509b9973f1a12056915e44440`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52fd3b2829a4a90396e730bb05b5685ca3e796a913593b91dda4cc283e5e8b6`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 99.2 KB (99243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1743a12c5b583262adb490179aeb5cb182f8fe9389663880f95527c27db067`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fca1206701ed80928b003456c51993e69bad74253efac7e0f64eed25375c7a9`  
		Last Modified: Wed, 10 Nov 2021 18:54:07 GMT  
		Size: 100.2 MB (100190494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8134f2eda537f35a9812d6e63e9b42b621503bf8e4f06a3027e74331c7e373`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 70.0 KB (70002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
