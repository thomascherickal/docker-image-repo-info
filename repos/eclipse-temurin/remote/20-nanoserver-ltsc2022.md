## `eclipse-temurin:20-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:e74368571821e94ad1220609fc0555cbf331bf1627a0fe42053a1c79fc431152
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `eclipse-temurin:20-nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull eclipse-temurin@sha256:5f7e51098e409c78129178a3cb78c24206a93d4e3cb98d1594c461f6615cc82e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.8 MB (317752502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa2a4ffee9b38a086935385c888c3871c07e12d9cab14e057c050532ceaef77`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 01:42:21 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:55:51 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 26 Apr 2023 19:55:52 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 26 Apr 2023 19:55:52 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:56:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:56:02 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:56:17 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 26 Apr 2023 19:56:30 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:56:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8058ec80ac2516d001291dea383d4abfa22416397a4c869e6fd79c0d4b64565f`  
		Last Modified: Wed, 12 Apr 2023 09:45:40 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffca90249d6eb4cb6932f602b2d42f8aa75ffb67722bb9a408463a5ed7037cc`  
		Last Modified: Wed, 26 Apr 2023 20:11:49 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90d0b38312fd1aec6dc2ec80892b3294c14ac28e33a04efbdde08699c62e9e`  
		Last Modified: Wed, 26 Apr 2023 20:11:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf6c055990cc711e478dfd33ce8143941cd912013b297dfed6b30358527a2a`  
		Last Modified: Wed, 26 Apr 2023 20:11:49 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b1ae52cc4723100150022ac4e94629f45df8ea7bfbe045e685587aec831984`  
		Last Modified: Wed, 26 Apr 2023 20:11:47 GMT  
		Size: 82.2 KB (82150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ed8ef3f78ebf341e9ebfc8e8242c616da4c739399f0eb766c4acc63f7af2b8`  
		Last Modified: Wed, 26 Apr 2023 20:11:47 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cb7e1cb36c05b2b41ecd5437a51c8ed4b7b0c95220cfa51037832b2c702596`  
		Last Modified: Wed, 26 Apr 2023 20:12:06 GMT  
		Size: 195.3 MB (195276588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b595327b5bf2a09f769f7083cf6b0f7287a1d126f62d11d26405835d09c790`  
		Last Modified: Wed, 26 Apr 2023 20:11:47 GMT  
		Size: 58.5 KB (58464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1077ba064e06a285cba87520cb619b7d78070f78ead9f84a0cb7f27dca4b970`  
		Last Modified: Wed, 26 Apr 2023 20:11:47 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
