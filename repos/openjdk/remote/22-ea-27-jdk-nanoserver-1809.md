## `openjdk:22-ea-27-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f6aacf021ae576f257a83709e943128e8d447c07f81d2e4e1a8d2095f6f9a560
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:22-ea-27-jdk-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:504c44b4c381c642431a31946d0678fb33cade7479c4349bfb57c43149823820
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305789007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cd80a6ee67ab1c0c50f1a8e0eeaa6f396778c075178364dd2840fccf54de87`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 02:19:34 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Dec 2023 02:19:35 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 02:19:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Dec 2023 02:19:44 GMT
USER ContainerUser
# Wed, 13 Dec 2023 02:19:45 GMT
ENV JAVA_VERSION=22-ea+27
# Wed, 13 Dec 2023 02:19:59 GMT
COPY dir:ff057bf08d63776ecb0d546e093c8fd881ebaf7ac625535f56acbf65c5f8c473 in C:\openjdk-22 
# Wed, 13 Dec 2023 02:20:12 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 13 Dec 2023 02:20:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e50e3f7d2a73e423821b8e25bb0f35f1fec64b87931b06ee30693c9c43d6cb5`  
		Last Modified: Wed, 13 Dec 2023 02:24:30 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5906ad26d23f58a45ceee721e7e4bd08bd7d26a01e8fb49fd19527c97f0fe4`  
		Last Modified: Wed, 13 Dec 2023 02:24:29 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d142c0668a0703122714079986d17eb84c5b04f7637cc81b9de33d6db36e532`  
		Last Modified: Wed, 13 Dec 2023 02:24:29 GMT  
		Size: 75.8 KB (75781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defdce6e8dfced70f7c99e6af49983cfb7bb94aae231556474106b214ab20e7c`  
		Last Modified: Wed, 13 Dec 2023 02:24:27 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d1ccb15e7e0ff20903afc7c23925223a0b3c29446635ce13f4bd4e1ddc82f`  
		Last Modified: Wed, 13 Dec 2023 02:24:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098aea5d7e94a717e7c54388a266db89bdbd58d0016b42db891633700e4e0d0`  
		Last Modified: Wed, 13 Dec 2023 02:24:47 GMT  
		Size: 197.4 MB (197352889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9985888df52d2dafe5339b97b24da785fc1317ad32727216721a7c12b26988d8`  
		Last Modified: Wed, 13 Dec 2023 02:24:29 GMT  
		Size: 3.8 MB (3843394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c9bc2dafa8b56be6147d3963eeb1ebd66d32014f6b751e841aa998c38c8546`  
		Last Modified: Wed, 13 Dec 2023 02:24:28 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
