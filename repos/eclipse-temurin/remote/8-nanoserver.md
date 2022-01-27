## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:0c27117c15fd9f502c7cfe993620e6f042c14196ecbcaaa7b678e65b13839b00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:8e45d4f53b5a583bdada23ad98751209d8d79940123b7728c03a7e9883519d44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.7 MB (217659737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892e3e13f642e94deecfa546353fd12683528b491acaf0f42268c8c2bc444958`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:40:04 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 26 Jan 2022 19:40:05 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 26 Jan 2022 19:40:06 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:40:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:40:23 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:40:41 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 26 Jan 2022 19:41:15 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a817cf994a6840d2ec1ca178f1b3a3d698844ac4574f0b200919dd32543473e`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78281d93367f9f44834a1cea97f2f673eefa08ace55bfef9b6d207b5fbdb663d`  
		Last Modified: Wed, 26 Jan 2022 20:24:56 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0132dc798046c5dc26d96480a61598a2a831ac0277d33369dbe3a349794b62d`  
		Last Modified: Wed, 26 Jan 2022 20:24:54 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bf88094cf7352bb6f443070265455423df23bd0ad44f53653faf4e3b89c989`  
		Last Modified: Wed, 26 Jan 2022 20:24:54 GMT  
		Size: 79.4 KB (79437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d7dcacc0b09ee26b8a7e71b2c35a0fdf50787805d36f6ee6c0d99594041acf`  
		Last Modified: Wed, 26 Jan 2022 20:24:54 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe3cc08c32047599ede5d1954faecfd72e22253fc3413c8fabae46387dfe8d4`  
		Last Modified: Wed, 26 Jan 2022 20:25:07 GMT  
		Size: 100.2 MB (100180227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b47669569d5d6f9ac60aa25a236fb6228bb0c3bd0a8ad4730786f047a6913f`  
		Last Modified: Wed, 26 Jan 2022 20:24:54 GMT  
		Size: 61.1 KB (61114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:600c9b3172a0deff43def203853a6c5e447fd106b32e89b42a0e06b16992f563
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203394924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11493a573a3d990da9fa116d8c9d6b2c77e494964c78a79a4b2b9f4e84c904a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:03:47 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 26 Jan 2022 19:03:47 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 26 Jan 2022 19:03:48 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:04:04 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:04:05 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:04:21 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 26 Jan 2022 19:04:35 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171e2f7c7a6e8f151d275f0c0d0e209a4f981d08cc54d67365a6bac9801a28aa`  
		Last Modified: Wed, 26 Jan 2022 19:55:38 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc51e82db88da446bddd34c4372063084f707f94b8194d18c86df0a4730c03`  
		Last Modified: Wed, 26 Jan 2022 19:55:38 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997fd90ba65911ba11cb51bb34e61bd1e257c896460b166276a9ea90251a19d`  
		Last Modified: Wed, 26 Jan 2022 19:55:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8013e6146c43f3ea2256a4b16a10cf418d4391d62f48d471e590c0f82601a89`  
		Last Modified: Wed, 26 Jan 2022 19:55:36 GMT  
		Size: 68.5 KB (68519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20e2ed329053a278483c36fdbda576b30f373d2c76d409e56bbad18fbbba001`  
		Last Modified: Wed, 26 Jan 2022 19:55:36 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0576ed43a5d1e7b5f3a06eb5aa6d145120876a4ac4107b91d9c1d7f92a50871`  
		Last Modified: Wed, 26 Jan 2022 19:55:50 GMT  
		Size: 100.2 MB (100185722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f991b4f6c22f1f51dfe10a642523bebd23ce96b5523c03e16b8a534096f3a03`  
		Last Modified: Wed, 26 Jan 2022 19:55:36 GMT  
		Size: 88.4 KB (88353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
