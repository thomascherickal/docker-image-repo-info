## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:543717e45397a0c84af960f684739f601fd981cd443f9d505a07a87977076389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:293284ac97f0ea12f350d4cf1acff2a9ec32d7b139551f59e9342d9811d336c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314719907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94e5a07f2ae58a4a195c22378149c116a0364470d324df50223fc1f53c842fa8`
-	Default Command: `["jshell"]`
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
# Mon, 30 Oct 2023 23:42:23 GMT
COPY dir:3378004dd1c559f9d7d6f4bacd149386aa6ab741f7dba391fbd8a10b1a80b205 in C:\openjdk-11 
# Mon, 30 Oct 2023 23:42:35 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 30 Oct 2023 23:42:35 GMT
CMD ["jshell"]
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
	-	`sha256:b2f68dae16207563c6dd6e328d01cde0b4f9129574554901c103a5f1ab6ac787`  
		Last Modified: Mon, 30 Oct 2023 23:56:07 GMT  
		Size: 194.0 MB (193969550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c524e3bd39274d83dc87b2f98d2b6fdd82d26a7439d491e2cf99e0fd5a564e6`  
		Last Modified: Mon, 30 Oct 2023 23:55:47 GMT  
		Size: 61.1 KB (61077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fc563093255804a6b8d517351510e805a5eab2662cd96b9e75080634ff0d3f`  
		Last Modified: Mon, 30 Oct 2023 23:55:47 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
