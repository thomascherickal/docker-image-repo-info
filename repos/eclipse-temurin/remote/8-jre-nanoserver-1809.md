## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:4bea30f6fc456bcbbd38e2ae692944daab4e0e34a5768ff03e490ac55531608f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:23af384394a9388fa3e51ddfc6c28a3caa1120d7de57e313b6453c38af55923f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142272206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2b00c835bfa2c722801b5d032d3a761eb446e9205a91cb592cdc9805db90e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 05:19:56 GMT
SHELL [cmd /s /c]
# Wed, 12 Jan 2022 15:34:02 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 12 Jan 2022 15:34:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Jan 2022 15:34:04 GMT
USER ContainerAdministrator
# Wed, 12 Jan 2022 15:34:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 12 Jan 2022 15:34:19 GMT
USER ContainerUser
# Wed, 12 Jan 2022 15:37:46 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 12 Jan 2022 15:37:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:71dcb756adb8534a87210067788d6aa4a5a366b72d022b7af035e5263a3e54a0`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9688a822af3207c76f479e1dcd24729a872b14ca7b578a5cf939c8da1beea82f`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9392e95e3451d5255c7eb6f7082ecb82e722cc977e6a4e482dd4f191928d78e2`  
		Last Modified: Wed, 12 Jan 2022 16:05:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff7ad2a002508b7608d2069eb80fd73536913d79f8a080b2306aaac7967151f`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d3d451d5b86383a9c3ed5b112c411d530439c1306c852d24920a9e3cc74144`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 69.0 KB (68977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3aacb454a880cd5cf940cca71b6570e6eabd1e99834bba212fef2aab817436`  
		Last Modified: Wed, 12 Jan 2022 16:05:15 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daca65f01f6a9f9fb3688564f2c3f4985892fe26352aaf0f2d8d1e76ba68729`  
		Last Modified: Wed, 12 Jan 2022 16:06:06 GMT  
		Size: 39.1 MB (39085643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfb18fbadeb0fc4302cc0a86ce6763afd00754d14c4f43ea926bf32f50f2267`  
		Last Modified: Wed, 12 Jan 2022 16:06:00 GMT  
		Size: 80.7 KB (80710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
