## `openjdk:jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:dde091693db4b483777372799cc843cb83b9fdaa5e437f7c6b6d410c92a9a067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:jdk-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:b8b926ef0e1e054e02a796bfd8d1b74addad1db4aaa923ec5c7a0e1227c6c691
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298476675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6438f9ab714ad8dd14392f7e557d3ca90b94f00d0c89c3af0b732a34ac314b23`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 15:30:41 GMT
SHELL [cmd /s /c]
# Wed, 13 May 2020 15:38:55 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 13 May 2020 15:38:56 GMT
USER ContainerAdministrator
# Wed, 13 May 2020 15:39:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 May 2020 15:39:09 GMT
USER ContainerUser
# Wed, 13 May 2020 15:39:10 GMT
ENV JAVA_VERSION=14.0.1
# Wed, 13 May 2020 15:40:02 GMT
COPY dir:ab773af63638ba53f65d54912a2b4baedee0f85fcd6e6a001a89287a6d7b78b8 in C:\openjdk-14 
# Wed, 13 May 2020 15:40:24 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 13 May 2020 15:40:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c597e8fceaeb76628095f6dcfa538d497e85739068a817b45d73be2b96a3b37`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff38cc37c53caac01d84ef5b2e9cb4e18f80e64c02df3f3934e4398d9c6a7c`  
		Last Modified: Wed, 13 May 2020 16:18:28 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d18c952f016fdee77f057d61b8ec6c10b27ffd4bdd465ab5b93c8911a821ea`  
		Last Modified: Wed, 13 May 2020 16:18:27 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa1fd38ed77d55ebaee0152dbc5c9338eac427e0dc91c7d54a0faec80c36faa`  
		Last Modified: Wed, 13 May 2020 16:18:27 GMT  
		Size: 70.2 KB (70232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8d0f9e82a386f0408cdd3928076e8235c121029c4684dea20ca09816e18450`  
		Last Modified: Wed, 13 May 2020 16:18:25 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313526f79d87fd63c34c4044bce8573bcceb4d53adb56272c9b7a27fb7b60420`  
		Last Modified: Wed, 13 May 2020 16:18:24 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248ab719a4f5258eaf8ee990f4b1c56762240e441f10cdc589863b309893b767`  
		Last Modified: Wed, 13 May 2020 16:19:04 GMT  
		Size: 193.9 MB (193937069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3164f8051a1c7ebcc35bb19c5cd3313397b4dd462a6d4a6711d0aa4be7fddb2`  
		Last Modified: Wed, 13 May 2020 16:18:25 GMT  
		Size: 3.4 MB (3444166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7ed2e2c561a43119b025fc571eacfef46fb1f86e46f6ab784ee20c3b55a801`  
		Last Modified: Wed, 13 May 2020 16:18:25 GMT  
		Size: 935.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
