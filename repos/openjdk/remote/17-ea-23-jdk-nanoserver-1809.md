## `openjdk:17-ea-23-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:fe59603f0c7c25ec206170bf22a90968e566448b1bb3aa4239a830b5f8b52cbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:17-ea-23-jdk-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:a65a628ba00a4afb258c77b356a956facfd58349898a1a25a91fde55cdafe49a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.2 MB (286178706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20c52c65d4ffa63f5ed2f8ff68ae4c590e5fce1ca7c523f313b3a494b5da1e4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 16:42:56 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:42:57 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 16:43:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 16:43:21 GMT
USER ContainerUser
# Fri, 21 May 2021 17:18:50 GMT
ENV JAVA_VERSION=17-ea+23
# Fri, 21 May 2021 17:19:07 GMT
COPY dir:8d8824e2772c7416e8e694dc48fa7cc8a6ebd74fee09915494cbbc4e6160029a in C:\openjdk-17 
# Fri, 21 May 2021 17:19:35 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 21 May 2021 17:19:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea91a7775c05d55a850a2983043468ce6ded7406743836cf8f33afb037aba1a8`  
		Last Modified: Wed, 12 May 2021 17:16:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0a5b4dd190af3527c02bb783babc5d88014a4de37555355c2f7a59dd21449`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab5fc14de7c93823ea1579b64e1e79017e9738a39e5d165aeed23c15bf7ffd`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954cb2ae96dfb0f537ce02738b91077c41cda7743ff097b99d8a6cfc74e211f`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 69.5 KB (69533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95581d66523cc5b44afdfbd1f1e7732689ad5d73bf1c1352ef8f1e669dceede2`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824ba7d42d3309871c67134668788f1588a1dad3aeca81da9338c91bd7a17f18`  
		Last Modified: Fri, 21 May 2021 18:25:16 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec2ca0537bb7df9636b4afa2355749354a2db574e2ef03b88a81016c02073fb`  
		Last Modified: Fri, 21 May 2021 18:25:36 GMT  
		Size: 181.1 MB (181091501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f5330d51ef6934dbcdf181dd0cfac91fcf7e32ddb01637065c3d4e2641154d`  
		Last Modified: Fri, 21 May 2021 18:25:17 GMT  
		Size: 3.6 MB (3635643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4de470a745f865b4ad2df9ceab8b27d8a182435c99645cef8f16b0dc351a47d`  
		Last Modified: Fri, 21 May 2021 18:25:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
