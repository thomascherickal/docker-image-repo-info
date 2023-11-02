## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:9e4a3791e02a295d4a9e1d12fa83f98e459b78ce3e8a851f150a8f5fcbeae40d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:4daaf5ae4a2c22df81a5e05cc07bac338cc09c98ad67150a65819fc2691271f5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.4 MB (222446707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694051b69d8dba55d0f62c08008a4368bc61ac370c76ae9b17deaba76bec163a`
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
# Thu, 02 Nov 2023 01:29:37 GMT
COPY dir:d9c44d909d2b41aad5bf6fa4f7c7d36e81063822ae5e7ef30e4851bbe7809503 in C:\openjdk-8 
# Thu, 02 Nov 2023 01:29:50 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:6b1a4d2308fcf3cab9ae8adac26ab6cd22e30bb61faeed1cbf18d5bbbd212658`  
		Last Modified: Thu, 02 Nov 2023 01:35:56 GMT  
		Size: 101.7 MB (101696221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece75bc3fe364391d82a78f12e16712b5e2d221323be33ba16decfb229fa1a93`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 62.1 KB (62090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
