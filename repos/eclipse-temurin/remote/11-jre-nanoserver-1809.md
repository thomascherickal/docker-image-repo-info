## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:e66ed94a2a57de84ef25c7a36b8eb15a5ed3c2a1df94dbd323ae6b2a76b6ed5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:6ada453a565e7dbfb4e00db092d0c1366b4224eef55a98e8f60b3205f9079d91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146102530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c69584a5582ff337312bf4e4a76ecfe34d63203334e2cfe29fd800915afb19e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 14:59:30 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 13 Jul 2022 14:59:31 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Jul 2022 14:59:32 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 14:59:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 14:59:41 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:03:55 GMT
COPY dir:b81e8d840693600453cb21437c037772b6cbe813879626cf7da1b40ae8a26737 in C:\openjdk-11 
# Wed, 13 Jul 2022 15:04:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a44b4109423f62e18da9164482c765f03b13a78c5d72b5d8d19fdf076b46c64`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3923d7358dff5064f6087c0c442b1878b2ac256f295e256dad48f49be8675241`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b4b5ecf5629dc3d0a883a559f734059e0adb86e4078f853a87ae86b008db3`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9585a652a462592aefc444c93997c7c3cf5a9b3129fec8879b5515613bf72380`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 71.3 KB (71294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71a31f96ef3a41839d79e6598b654d911e1b0c88598b4d2f29ad83ed0b4139`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293900609d55422661754a4324d30c8b3839f696625997f80163c3bd06bcf38a`  
		Last Modified: Wed, 20 Jul 2022 12:47:44 GMT  
		Size: 42.8 MB (42787281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6872245f79d0c974996458f6e6197c9e376dde4b9983e146ce85fffaf8babaf`  
		Last Modified: Wed, 20 Jul 2022 12:47:35 GMT  
		Size: 83.2 KB (83172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
