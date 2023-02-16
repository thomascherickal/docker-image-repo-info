## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:3e7e66639b4b77492f39d8ea971d843c7611209fb1ba28ddd85c17871ce04bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:4d8e28bb16b17346e36d7e558d250b52b68e00ae9b25802b246f9ef3b50cf83e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162200306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed935f47e78a7cec1765eac7f6e3c749a7722f4ab8b5972c30c76a11644c184`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:34:04 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 15 Feb 2023 23:34:05 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Feb 2023 23:34:06 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:34:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:34:26 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:35:27 GMT
COPY dir:dcd2674e91fb412db18990a7004f7a484148b702bd6de08f5ae3a3d6f6a3f6f8 in C:\openjdk-8 
# Wed, 15 Feb 2023 23:35:43 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a35c9fffe8173c13d87bf21f7de2163ad9db299c1f8071c714dbce581312486`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b632c77d3738a4b0bd36ae23404bf676ce2b151ee71067572209262a0d00369`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cffb264ffd2903e1afbd610e16e75f6727340bc7954f9b679953a0bbf10ea7`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114660912ba2c4f3763f99ae68083aea983bbb7f7e0ad4a0988ffc5908f671a6`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 85.2 KB (85222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a0038a4b64f24aaf7e4ddd119116fbd8796a8a7a59946faab0d2cc474b2f7a`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddde13998c5834573c3cdc6b685e81ecf22249210cc7c324f25d6cbd50380ad9`  
		Last Modified: Thu, 16 Feb 2023 07:21:38 GMT  
		Size: 39.9 MB (39929287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5b8e4e11c1e420ac8d770798a5007138aa3f868f579487a33980a7eccec575`  
		Last Modified: Thu, 16 Feb 2023 07:21:30 GMT  
		Size: 60.9 KB (60912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
