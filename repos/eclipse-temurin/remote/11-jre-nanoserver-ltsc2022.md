## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:a53ee8763ef77598535395ebb1458b679ef294f6eee92068ef92560957535afc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:f136087ba6b59ea3ee5996fe99a0d2517a07401fb256931f2643d7584dd28ff9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.1 MB (164099686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1908099195efd54a7b821e0412960bb9c61af9802f54efd67b17f495812bc55d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:41:57 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:41:57 GMT
ENV JAVA_HOME=C:\openjdk-11
# Mon, 30 Oct 2023 23:41:58 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:42:10 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:42:10 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:42:46 GMT
COPY dir:32725fa0f7edeee10e8937816f70b588636369ca6a0eb68560cc5c3b2b3f76d9 in C:\openjdk-11 
# Mon, 30 Oct 2023 23:42:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:ea2e6c4facc55dcd7ca1deca5746b9c9d158bdd0e471a094e15c3b739e14a803`  
		Last Modified: Mon, 30 Oct 2023 23:55:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d8dfc460e5a00f1638d9c6954cefd01eb5c6beca2fd650431a9270a04dd6d9`  
		Last Modified: Mon, 30 Oct 2023 23:55:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435d22be431c803484321d84d9f52758cf72f6b7852b4703a97ca656f8c351b7`  
		Last Modified: Mon, 30 Oct 2023 23:55:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506f18ada228dd4d2b3a478dc958f6c68a3274501cc3b1ebe82ec3a210b580c`  
		Last Modified: Mon, 30 Oct 2023 23:55:47 GMT  
		Size: 78.0 KB (78029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8220e72830c3155eb6e7ecab6ed20ea660f5dd0c82c7654432a261db319d4a14`  
		Last Modified: Mon, 30 Oct 2023 23:55:47 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9933b83606d88c2b1867d031fc4df7f04b8bea203ec315abd7506c6191c26fb`  
		Last Modified: Mon, 30 Oct 2023 23:56:29 GMT  
		Size: 43.4 MB (43350480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6545a90a9710ea1a2eda7a61a7ab0e3c1af90626d65f2a76df1a5205813af571`  
		Last Modified: Mon, 30 Oct 2023 23:56:21 GMT  
		Size: 61.1 KB (61083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
