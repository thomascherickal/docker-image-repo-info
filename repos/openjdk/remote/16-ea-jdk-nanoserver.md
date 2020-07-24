## `openjdk:16-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:f40d23e54320c5eb5454e2f4343c2c9d6cb2e8f315dae31dcddce0f964a23bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:16-ea-jdk-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:56dae64f9b207b92776d71f9b83267f729effb19639347788aa808e5aafd5a93
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.5 MB (296497276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e43c8a14d528c1587494cda71c8a135b77083a9136db4d8a8fa4f34f5295581a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 01:54:44 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:54:45 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 18:21:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Fri, 24 Jul 2020 18:21:02 GMT
USER ContainerUser
# Fri, 24 Jul 2020 18:21:03 GMT
ENV JAVA_VERSION=16-ea+7
# Fri, 24 Jul 2020 18:21:41 GMT
COPY dir:03818c511870237d8b8a45f04c722372850f9c70fc5bb0a934f338db9972dc32 in C:\openjdk-16 
# Fri, 24 Jul 2020 18:22:05 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 24 Jul 2020 18:22:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952f154db0b1aa57586a649f933acc22620a18dc11bfe0f2369af17af77fd616`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d574471402fee7c0d2fb574eb4bbfd848f720c971dc4d9318a7437da54d1ee`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa94d52ff38f89a9e35647ee58e1b9d5c1ee9f238d17d1d94d294263683a8fc7`  
		Last Modified: Fri, 24 Jul 2020 18:34:41 GMT  
		Size: 65.3 KB (65316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70146e6967d5a15f9a4884bb2688dbc7af97e64172e951cc00ccbe779da256fe`  
		Last Modified: Fri, 24 Jul 2020 18:34:38 GMT  
		Size: 822.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b42b1832c151e02b00de5adf1b557d6eddfa5baa624a710927642054df37758`  
		Last Modified: Fri, 24 Jul 2020 18:34:38 GMT  
		Size: 823.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4295dd45fd21956d18dbc7ac1f39929eb051a73e88e35be85003ad82ac269d6`  
		Last Modified: Fri, 24 Jul 2020 18:34:58 GMT  
		Size: 192.0 MB (191999541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4faa95c7d4eeb6795b7d597aa024f2d40cc755a305722e00a6a4f5f13a9357`  
		Last Modified: Fri, 24 Jul 2020 18:34:39 GMT  
		Size: 3.5 MB (3531697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10da4a21915486fd0d376b1d91897a532a7ab3aa854cac2c794377af69934dd8`  
		Last Modified: Fri, 24 Jul 2020 18:34:38 GMT  
		Size: 817.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
