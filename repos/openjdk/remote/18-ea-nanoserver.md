## `openjdk:18-ea-nanoserver`

```console
$ docker pull openjdk@sha256:08750e4c0d4c43b166168451beb978526cf2051a6d5bd4cf743c0f23dd1716f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `openjdk:18-ea-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull openjdk@sha256:60f87f66b71964de745fe7029d3b0f61cf354439aac38eb2a22fb60abb580b17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.2 MB (290203682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ef2b493b84d187bdfa482311ccc0affe57b0f3fe3e1f670457ac3a83e8a1b6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 20:31:55 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Nov 2021 20:31:55 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 20:32:07 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Nov 2021 20:32:07 GMT
USER ContainerUser
# Fri, 03 Dec 2021 23:13:45 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:14:02 GMT
COPY dir:abb835dffc632d332fd17a30ecdca265103ae97699403dd16609abaa35bbdd81 in C:\openjdk-18 
# Fri, 03 Dec 2021 23:14:24 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 03 Dec 2021 23:14:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e60ec86b90e1492e0e0ed2cbebcf624990a34862e24207343fd85b84b3544c8e`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d97d878bac5dd9dcbe1bb5f45ade2111fc77e8d4a5a348163bd9c3ddddbaf0`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a46fd95d3a8e8b5949c49cc0d70b858bddbe38c8c33e0a6a3e0f157d7795a`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88539ad3f1fb0ea6957da9a7298c1f6546afbb52b2deb7199763195fca993d98`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 74.2 KB (74205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d133fe2173015750539b2d0a8fb86dbdbe0c6b44c8d75ddeb714a82814f98e00`  
		Last Modified: Wed, 10 Nov 2021 21:11:33 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0f3f851c2a3742afddce90ddd453850f51e044bf09439fea7b8d3b1d7c2ae3`  
		Last Modified: Fri, 03 Dec 2021 23:37:43 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d90967e75fac31f66b52f7b21194a0435c417d1e916ecccbb11ebe36a9cf23`  
		Last Modified: Fri, 03 Dec 2021 23:38:02 GMT  
		Size: 183.8 MB (183810844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5219c17ef5ef5a6d3dbd45dc180d93691a8e4da907a6b940a9d68163587fdc64`  
		Last Modified: Fri, 03 Dec 2021 23:37:44 GMT  
		Size: 3.5 MB (3528820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4f2d3c6acad41e0dd656529844cafcfba7a06e020e202234e495446a9d5b69`  
		Last Modified: Fri, 03 Dec 2021 23:37:43 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
