## `eclipse-temurin:20-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:9fc1faf9186c36abc5af3e683f7f753831b7c6bff40d257b7505e1743f71a396
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `eclipse-temurin:20-jdk-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull eclipse-temurin@sha256:5c09faf60bd10698f0da6f8b0b022b5e9be8e265536396526ead117e71bd43a5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.7 MB (303731824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8310fd10f8a335dae6743f2118e35034b891699b63b36035ee4ebef146f1a925`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Mon, 24 Jul 2023 22:29:10 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Mon, 24 Jul 2023 22:29:11 GMT
ENV JAVA_HOME=C:\openjdk-20
# Mon, 24 Jul 2023 22:29:12 GMT
USER ContainerAdministrator
# Mon, 24 Jul 2023 22:29:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 24 Jul 2023 22:29:26 GMT
USER ContainerUser
# Mon, 24 Jul 2023 22:29:41 GMT
COPY dir:4ed074865171ba014f3c2f68f57ad2bb21a4dd6e4cf7ff9654ee6c4c6e5176c0 in C:\openjdk-20 
# Mon, 24 Jul 2023 22:29:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 24 Jul 2023 22:29:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3304d99bb45bd396562f7f91d37af5a446d4889b089704dd94525f599a313b5`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a234201ab08724053de32e2bb25598862ec6eead6ec84376abe96d5f5bcceb`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced14764f8bc8c1a02eb2929b520cbd53bd6a49cb6f9126918c7c487b27966ba`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1db76a566fe492ce96b9e5d4d6ec9ebffec2219c549c0f580ed3b301d86e49`  
		Last Modified: Mon, 24 Jul 2023 22:40:18 GMT  
		Size: 69.1 KB (69098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f620e23904692174522ca4e362d9121e805c30bd6744dc90a68dd2c5f72f6ff1`  
		Last Modified: Mon, 24 Jul 2023 22:40:18 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c787b8395272f9b95f7f0dca93395c8a223bf0016e643fec7f3f366c34d819a`  
		Last Modified: Mon, 24 Jul 2023 22:40:41 GMT  
		Size: 195.5 MB (195465154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3326d75a63976dbe00de11bcb95f641fa615ff402bcfb4431cc166d4582758e`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 3.8 MB (3782440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d5a2e9e8ed122257c2ee6125fdea981196ae213c72be97efce0792a554ae3a`  
		Last Modified: Mon, 24 Jul 2023 22:40:18 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
