## `eclipse-temurin:8u382-b05-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:cbce6e14b6991b1cfad838bd3051c9eb564d8be473f294ed5e2d4447e2e1ec96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:8u382-b05-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:e76aa91db2dbe9d85075a1f23e3f4b79a604471b0b82274513c35d9e7375a310
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160739833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7f4dba44195b5742d8554526523a9059897f9fa3b802e2fd15b10b99a721ed`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 02:14:41 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:14:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:14:55 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:15:28 GMT
COPY dir:f24575d0fd9e2979f5a8010c202ec6d963a3eb3cd788517e3ab1d758c8e6ad81 in C:\openjdk-8 
# Wed, 11 Oct 2023 02:15:40 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:9e573e8d27715408942370bbe3e31eb4ae2c5feadca2cccb3f642115eb3782d0`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a95305dbe93fdf5eb7909af77dfe59c82075bfa61c017c8df26328dfd9e91f`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfa1af4fca27ac3e9a84f67da56ec595a2803fbb10b8a798ff27458de06a3f8`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe98fb9ff1cdb5c208cddc16e8f295fc8a2f2c4015171e38254517402041f9b7`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 86.2 KB (86233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1c6eb49fa819be7d62d2c434696a6dc3cde2b7a8d4494aceae0bc0c7739b2`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a267401df6ca6ce1b2a12a5ae3792028abce2a246a07f2590ed80d0025cda`  
		Last Modified: Wed, 11 Oct 2023 07:30:02 GMT  
		Size: 40.0 MB (39981269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8201ff253dc64f4908c06b287b40cb6e82b1a8e160fb56ce643ac1fd39302c`  
		Last Modified: Wed, 11 Oct 2023 07:29:56 GMT  
		Size: 62.2 KB (62226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
