## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:39efd569f3490badd5510e5efebdf40c3073796c7a85ac51c83de7321b0e8f37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:07749e4562b0e0758918a21839fcf9b4cd89f8b73c1e8bc2f70159a911fd4d8b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145945279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a88dca3bafd333f6fa613865fff4a83423023532ce890057d635277e92871d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:15:36 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 26 Jan 2022 19:15:37 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Jan 2022 19:15:37 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:16:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:16:01 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:21:39 GMT
COPY dir:6031cfac1e4bd8de6c5533bea0aabc25715779d854db7f41b8aea3e1449ff0bf in C:\openjdk-11 
# Wed, 26 Jan 2022 19:21:51 GMT
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
	-	`sha256:123ab2ee14a125bf4b0c6cbaa7024d6fd79d88b72564d3f5ffc2a991388ca55d`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a2e9edcceaff9bcf83e6afe158f5653cb569791bf57461c14bb12dee4c4f4`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd6c39c776fbc28c7dc393f112bb0ec49b97e64c79c5001c3b4c9067461568`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5ed98fdccc969f48e18c637043dc0f01001d2592b60ead2a792c7d37dd616c`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 75.3 KB (75305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c4cf8478e4d4c0f8a13f4a6039564552580a3c553158a2405cac2386232588`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77839c10f33b8e951d6fc909e7fef33f9cd4c48d319bb69d796fb53e6eac5d78`  
		Last Modified: Wed, 26 Jan 2022 20:07:50 GMT  
		Size: 42.7 MB (42730915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e6bca5f7ba87b483ad58ff7823714793944552ec25249fa6bf2b3a4173d02`  
		Last Modified: Wed, 26 Jan 2022 20:07:42 GMT  
		Size: 86.7 KB (86738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
