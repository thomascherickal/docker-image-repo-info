## `eclipse-temurin:8u332-b09-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:c68cdec80f4418490ebd0f4e427d418ed74f9929214e21b5dc3ca77b44e10c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:8u332-b09-jre-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:ce589ef6e18490c85ec021111bfd65eaf7bf2284c4b9c4f7d4853cb7a2c4b71b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157318354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9329e92238595d5ddd351052a2f146b546e8e4bd98a51a4e732c6a1c4223b6c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:22:06 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 13 Jul 2022 15:22:07 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Jul 2022 15:22:08 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:22:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:22:23 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:23:02 GMT
COPY dir:3ac3da968b0a55dd3b56d678ae78ff2fe7435f143b42a50fa75d097fd864892f in C:\openjdk-8 
# Wed, 13 Jul 2022 15:23:15 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:569505cbc9e1bcad1fbbdd7edca170e5a914864bcad2f53e1fc5d5816ecc8aa5`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e753c6d4dfca51a49dd3fc56974f087597e367a793bb5f2c1ef005a38bd1af`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5976c511319c85af2c0a6b577889e9d3f37bfba7a6a3808b327593b8530df6fe`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b0804d51dfef1843793b7fb2b1f2144a86fc3df1189504f0ce2b47571059e2`  
		Last Modified: Wed, 20 Jul 2022 12:54:10 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95fa4129de0073ea928310c5497796ef7f31013bd9ba794c79a0fbcb473e293`  
		Last Modified: Wed, 20 Jul 2022 12:54:10 GMT  
		Size: 76.3 KB (76317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5aeaa88ab2381bbf369afed6166f91a40d741f286986da56466c8975301640`  
		Last Modified: Wed, 20 Jul 2022 12:54:10 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b432c8ea5a086b9720533d0fb4be2d12542fd4b319f06e573fee883054aeffe`  
		Last Modified: Wed, 20 Jul 2022 12:54:45 GMT  
		Size: 39.1 MB (39129239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0398add5694acd1489e3f26199a742a28497bdf37ba6978cef959dbf333d1879`  
		Last Modified: Wed, 20 Jul 2022 12:54:38 GMT  
		Size: 60.9 KB (60937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
