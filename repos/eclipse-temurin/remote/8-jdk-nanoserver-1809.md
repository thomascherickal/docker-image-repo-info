## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:df284be0b96f117601529b9a8910f13f61de5ab7ead0d987fa2a4e90dd21b931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.5206; amd64

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
