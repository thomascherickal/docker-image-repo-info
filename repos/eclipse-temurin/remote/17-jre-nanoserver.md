## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:aa00337bfe2a562d1853a2100fc831a39691ed218da238aec1c9b65d12de60a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:3b648edcec4dbc9f22c98ff2227c3a8587a11033dcc0f253e73a6e1bee8fcf3b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160577739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561d87822dbfc01d1202323d0da28fa5749bb145b0a56a838ae174807c4b68bc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:43:57 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:43:58 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Jan 2022 19:43:59 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:44:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:44:14 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:45:22 GMT
COPY dir:38eebe4e3a4da98e178f49482de333d171d427f5886e68b2b67715641b9694d5 in C:\openjdk-17 
# Wed, 26 Jan 2022 19:45:35 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774536782c1c4d4015e8359ac0437fdb94a8d696f9cdef5e9936e721b99ae1f`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12214b1befa142979cea977dbe18e01fc824195c2dd83727fa5b15e41c38638c`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff8a2a945a4d41d4a21c3e74b99a007be23a149c47ec52f2f33ddf270bb6f16`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ada735cfb773a4d0ed93bd8768bcc1e11e8f13d0f5e8ebd60b41a1cb4c9f8`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 84.6 KB (84623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf9b071a062772e3a9bd393d34c0fae1dd2444a5298988e86b1daa21b0f785c`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2ac933ed9e13c571120b9d64174225b8fddc00d264c48a751ae8bb7f6870f8`  
		Last Modified: Wed, 26 Jan 2022 20:34:45 GMT  
		Size: 43.1 MB (43092394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05696213a4898846852c943181f4e0fd8d3d61bd912e2fe8f1de99b22111eb9`  
		Last Modified: Wed, 26 Jan 2022 20:33:54 GMT  
		Size: 61.8 KB (61799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:8f7296a465ab4fd77eebac8dac2c3c241c98c45dd19cbac7d2d9fe5e904c7672
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149213824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f22850b422a42c5e84f05f92e690bf467e3ada7129144e4d88662788795d82a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:33:37 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:33:38 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Jan 2022 19:33:39 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:33:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:33:53 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:39:40 GMT
COPY dir:38eebe4e3a4da98e178f49482de333d171d427f5886e68b2b67715641b9694d5 in C:\openjdk-17 
# Wed, 26 Jan 2022 19:39:54 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159cc5ffca5107ce551dd80b9ed61ac450096630236c2247dc99f8d116f541c`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e919bba1969715a875c8d96965c2d78e044605cda42fcba99d9ab5f5a94e2976`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca96870c535b980f31c3d23beefcc204f3b3be6952024caa9e6b6a3caa8b8c`  
		Last Modified: Wed, 26 Jan 2022 20:17:22 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2c81986540337ad2bf29c07de92b78dd583bfbb3a00a3e92bdd0714f9f8b29`  
		Last Modified: Wed, 26 Jan 2022 20:17:20 GMT  
		Size: 68.0 KB (68032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b57584fe1a0c2ff5aa5a8ed4aafa3786359488ae67aff438b6fa1e4e3cf31f`  
		Last Modified: Wed, 26 Jan 2022 20:17:20 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220c8966757c4211cdd75f0b6e0a8c07f053f75c0bbfd541882d97f0b2012e0`  
		Last Modified: Wed, 26 Jan 2022 20:24:44 GMT  
		Size: 43.1 MB (43072462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92be6f9d26e8310c6921ce8c943c6960a7267ba6871317bf45b9ff7b29c9e4ff`  
		Last Modified: Wed, 26 Jan 2022 20:24:35 GMT  
		Size: 3.0 MB (3021033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
