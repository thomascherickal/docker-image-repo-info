## `eclipse-temurin:17-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:a6de50fae029326413d8f3248aded1e0bd3fbf50fdc3a8bb116d0c2d77c0bb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:17-jre-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:ad37c1578b294ae0de93d8d8c95a3988bd90bfaeca528b88ed9536e0a8ae845a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.3 MB (149276962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e059022402ca0d44ff6530bd34d9a5c92a5346940ec9b6db34583b7e248a6c8f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 21:56:20 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 08 Mar 2022 22:20:40 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:20:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:20:54 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:25:34 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Tue, 08 Mar 2022 22:25:52 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e0065cd23a657c8f30ae5af121fd18451d2307835a1124ea57c80683eda26c94`  
		Last Modified: Tue, 08 Mar 2022 22:37:21 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e28e0120ae71480ac4b5292e1011f3e9a68e7648b992c086019524244ffc7f1`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d91688edda3231dbafc3286e5ecd7bcc1653c6a0e16cc01372b62928a409ef`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2195699d328d0527e400e78f2794d1150c371b24ac84f8bf12bba4aa47e9c2`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b8d01d40707a79981646b757c4bb673b5163d48f0f7e69f846dc526b2f5236`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 72.2 KB (72220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759cdd0f2650d033acdd0769c7ca2cf4ab535325556e99d303605abfbcbaccb0`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6712357b9729becd822b87483e767eb39301f51f44a5b550551dc1b0b2d04a5a`  
		Last Modified: Tue, 08 Mar 2022 22:57:26 GMT  
		Size: 43.1 MB (43111671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12c3ac61f7e11bec955fc793072cdd2d1b05c809cd8e5dd47f731f59d1b0d0a`  
		Last Modified: Tue, 08 Mar 2022 22:57:18 GMT  
		Size: 3.0 MB (3032812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
