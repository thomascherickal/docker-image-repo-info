## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:4f3cae1e70f7eb7c5bac2ae832c61e7d223d4a75b093bd358af4aa66f2472f19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:765ceefa37926c8cabba7fa3445040826b92ee030025e63cf7fc0f1703372bd0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156563836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bc9704d8425fe02975b48538eb3cf413e023a099743100fc3f96a744093d0e2`
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
# Wed, 26 Jan 2022 19:41:30 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 26 Jan 2022 19:41:47 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:696732eaef9d4f3b73d80ecaf005dc4c78e71ad14206e3328a019d2b5f4feb95`  
		Last Modified: Wed, 26 Jan 2022 20:25:29 GMT  
		Size: 39.1 MB (39084334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da8fa16675f24a7f0117279ad42a83845a579a8317c593364f930ddf353009`  
		Last Modified: Wed, 26 Jan 2022 20:25:22 GMT  
		Size: 61.1 KB (61106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:6c9e0726828341e188e39c305ea664126fc46c07117b64095bc130557f6e1ecd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142285842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678a7c130f0f574b2ba1304f56bd291a5febb64eb05d054d6adca2513de6e094`
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
# Wed, 26 Jan 2022 19:09:03 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 26 Jan 2022 19:09:17 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:27218da284a9fe22a35f4671d7e396b144479270e8eaadf253eeca98380e50ac`  
		Last Modified: Wed, 26 Jan 2022 19:56:50 GMT  
		Size: 39.1 MB (39084550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d7dffb76efe4d5bd8f5da27d688fc4ab009e4358f9b6d5447bafe6706e0add`  
		Last Modified: Wed, 26 Jan 2022 19:56:43 GMT  
		Size: 80.4 KB (80443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
