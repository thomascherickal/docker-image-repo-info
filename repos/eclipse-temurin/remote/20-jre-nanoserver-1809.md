## `eclipse-temurin:20-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:f156220daae4fc336dd85d7503daaa3251bb82084a713ca676fbe8a8a1a50130
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:20-jre-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:2ab287f284973fc30f277beda08a436577fc72c95b41dc1a5d14eef567be1e4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153554348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f6d327b29776eee3ceec7cb6bb3716e450e218b3d2d9650455c7bc86e3a534`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:08:43 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Wed, 11 Oct 2023 02:08:44 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 11 Oct 2023 02:08:44 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:08:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:08:54 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:14:21 GMT
COPY dir:7e69bb3960973ab39fc2ba0552343e70b32506a25a841e69600e9c49be1d11aa in C:\openjdk-20 
# Wed, 11 Oct 2023 02:14:31 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:8b3995660243563f73dbbc84e0b91410b46a7c1da60b14695abe81d0f1496613`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b88d447d9eced836942706fc967433d907a7092251487a243c8ba882032f97`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c772bbcb4835613302d26f7f49700ec02040b02add8d519052c21a7c3aadab`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedee8fa0cf60903a52e89de725fa0b1bc5a681e4ce44b9b9d21572d9dda0017`  
		Last Modified: Wed, 11 Oct 2023 07:28:09 GMT  
		Size: 68.8 KB (68785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd66ef872b8166772391d501b081b022d73c0d160055f785613c9f690c08fa4`  
		Last Modified: Wed, 11 Oct 2023 07:28:08 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027e103237e2f8fc35c1cb788f1fdcf561d77261f2a71c72413292026cddade8`  
		Last Modified: Wed, 11 Oct 2023 07:29:25 GMT  
		Size: 45.9 MB (45856574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c352df5e57d91c2c3b4a00294e9ef8e41afa6aabfe1d7034e2e3c80a797ecb5`  
		Last Modified: Wed, 11 Oct 2023 07:29:17 GMT  
		Size: 3.2 MB (3158690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
