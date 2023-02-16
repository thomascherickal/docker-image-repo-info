## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:654445b210ad3a671d163b3689f3871e021aade34eafd03239e7b155a69ea07f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:3d6db7be566c6be4d7e646610d8148c1d0d035b60dbdcab35b4c7e45c26c65db
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295851387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6ea94c0072195970598969b2d3dec9aa7b52cd8f790db3e1ebba8914605dd0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:13:50 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 15 Feb 2023 23:13:53 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 15 Feb 2023 23:13:53 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:14:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:14:06 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:14:21 GMT
COPY dir:b9d1887161cde3cc24ae2101d8a284bfc20814b15fed427bc1c905c1248fb0bf in C:\openjdk-17 
# Wed, 15 Feb 2023 23:14:46 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Feb 2023 23:14:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5047e7d94bb2e815892681bc1c2cc0e556c3908e3cc445eaf8ef1bfab768b75a`  
		Last Modified: Thu, 16 Feb 2023 07:15:55 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c9d9e63980f86f4748ad41ea364243fcdd2030cbb5c2fbf0f3e6ffba161509`  
		Last Modified: Thu, 16 Feb 2023 07:15:55 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2d76298d022bcf8120558f166e636b0b40858d070b89222c516288eab20aef`  
		Last Modified: Thu, 16 Feb 2023 07:15:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f770c6b3e4ceb6df5edc9c113af9471ff5b0628c37194327a53b356d2368113d`  
		Last Modified: Thu, 16 Feb 2023 07:15:52 GMT  
		Size: 71.2 KB (71238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82366ce1aabd5306360655f80292477c00d57298c890c719818531c98e85f7`  
		Last Modified: Thu, 16 Feb 2023 07:15:52 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b3f6ec2521a8a01fad06add729ce34d20ea8e649f24fedb10b333b2dbc185`  
		Last Modified: Thu, 16 Feb 2023 07:16:18 GMT  
		Size: 185.5 MB (185467353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c0d7cd24eff2997e62d3e2e2bdd822682370eca1d59e27b079bed5b49537`  
		Last Modified: Thu, 16 Feb 2023 07:15:54 GMT  
		Size: 3.6 MB (3630962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88612c377da59cf8192b17dec259e88c28a112686e8581df1cfee327c6479ef8`  
		Last Modified: Thu, 16 Feb 2023 07:15:52 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
