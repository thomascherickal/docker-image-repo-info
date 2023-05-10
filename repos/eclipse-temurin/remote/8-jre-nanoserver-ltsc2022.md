## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:d5b091cc5a05bf12fd9f01f52002cea98b6092768bd4711651a82aa149e1265a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:494407580e60472443371e87c877f5f2fbb160f6a0c6fdd4dd7066b115258db2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160098325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715241fe081cdf4d31fde58dd2f92721e6744a1fcff3dd588a645aeb4087a82d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 12:52:54 GMT
RUN Apply image 10.0.20348.1726
# Wed, 10 May 2023 01:13:54 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 01:13:55 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 10 May 2023 01:13:55 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 May 2023 01:13:56 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 01:14:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 01:14:11 GMT
USER ContainerUser
# Wed, 10 May 2023 01:14:51 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 10 May 2023 01:15:02 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:7d382efe6974b94c05000b6a95c1fd28e1b8bb3e81cc4592b2aa1cc46b90192c`  
		Last Modified: Wed, 10 May 2023 01:48:23 GMT  
		Size: 120.0 MB (120001338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cfc306feea2a215b4a83a66480231042a4bdc8001d07d634086f52f1f5ab3c`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094733d5dadab2bef8ab3368427e514ab7e30f25fd583e7f0b79e1211370a26`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412fddde1681c84b2b6a8927173afc2fe9f93af018bce16dc94aba6a8d607f90`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227787a081ea4e59e27ad44da06e67980f31d6d33f0ad0cde9d223b1922eab27`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb1da43198006e4e845e7bf1fedc9f9ba423bf9b29f4e1ce47219bd03e2218`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 74.2 KB (74162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ecff3816dddd3fa41f2288c8e2d63096dd317b3032ff212861de09a424eadd`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699808bf398d6b75178eb7adbf93e390a88e77cfb76acbe29a56d4e6527f3808`  
		Last Modified: Wed, 10 May 2023 07:04:34 GMT  
		Size: 40.0 MB (39957886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdcf6c8f1f5b27eea70c4fc14804782ed62b55d56796fd8e59b71c099a8d4d2`  
		Last Modified: Wed, 10 May 2023 07:04:29 GMT  
		Size: 59.6 KB (59647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
