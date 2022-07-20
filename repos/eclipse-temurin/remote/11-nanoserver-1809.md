## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:dd2aa2fbb49d50ab92ec0cf80b772ceb6fb9dc01be473b71e11fa92655bbb00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:4698a5b89c8ff6b8073ca66ba3f780e3b3621c9b7cfdcb5263f8e3884a236a98
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295551018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb085db147ac9ae554b34122d9c0b1e50f750462b30e70de26baec5acfaacb`
-	Default Command: `["jshell"]`
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
# Wed, 13 Jul 2022 14:59:54 GMT
COPY dir:1583ce76f01a2d0a0742f7b70646c210ef8c619565a381c37e5a1156f6ec4636 in C:\openjdk-11 
# Wed, 13 Jul 2022 15:00:10 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:00:11 GMT
CMD ["jshell"]
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
	-	`sha256:7f379ff9eab2500a0d58433fb57c9a956b52ebfb30e35102788c3604cfcad26b`  
		Last Modified: Wed, 20 Jul 2022 12:46:39 GMT  
		Size: 192.2 MB (192225486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0eb5c38793a4e491a01c8bacd2bd71269893e245fc7b4d7bdc4f4d1cfd716d`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 92.3 KB (92289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd353facbb4da66e7e4884980ac8c974c815b02d6cc842a0de46ad598e9d15`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
