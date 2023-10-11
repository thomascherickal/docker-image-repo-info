## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:18cae32e805a1eb62d7b516bdc71e433d4b6f487bc5448e836de16288b699f43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:d2b842ce979128387707f05fd43c58489d4fe372d05e8e7161394ec68747942d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206100370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddddb6b6ea40716ad90c62b7964c04cabc57e6c3d43d297f4955cd10a058000`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:39:37 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 01:39:38 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 01:39:39 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:39:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:39:50 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:40:00 GMT
COPY dir:809f08e9d949f52aad6441d5338932efbf6208a06192d58db41d3e3c11ba3f9f in C:\openjdk-8 
# Wed, 11 Oct 2023 01:40:12 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfa6f4a1c2a7c533d18ec0dca92bed309d0669d2afab455d6d5212351b975d7`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170446211d70073742ac91df84068c411612746e25962e9ff96b3e9282f20ca6`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03792e6d164d8cd335567497987aebb8b5b2425e1cddb7bdb44d32a94149ce4c`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa70d1de1a8dca6152d4582a2933b41dd7345f53273a4973ce1d623209c972e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 68.5 KB (68544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d097244be50912160bdc8158894bd41a8b5cc337313348edc3b35420ac656e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1a28ac6f682938efb11d62c52c947c7943353b1afcfef288470f6742a36722`  
		Last Modified: Wed, 11 Oct 2023 07:20:29 GMT  
		Size: 101.5 MB (101480219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5631c9fa21ac32ab5ac29148be556756347ccae1fbec09d7500ee00c3a083460`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 81.2 KB (81233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
