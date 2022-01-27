## `eclipse-temurin:8u312-b07-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:65e76bdb8f650594b9df86fccfd2142d9d7ef23dc9b1e18aae73c6e59399af5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8u312-b07-jre-nanoserver-1809` - windows version 10.0.17763.2458; amd64

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
