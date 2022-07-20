## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:52d47cba7158cd6496345f824c1bb8d33e18e36f8cb6d2b3fb9872240334b28e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:043d4f3338ae62cd64d3a73c2f594585137593917891d953e06fe59725855393
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203389144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56121e78fc4a4dc9ed14cf156cc1914d9a4fb76d4c9377181d8bde8387a18a5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 14:50:41 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 13 Jul 2022 14:50:42 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Jul 2022 14:50:43 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 14:50:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 14:50:57 GMT
USER ContainerUser
# Wed, 13 Jul 2022 14:51:06 GMT
COPY dir:fe4a23cbc3aecb3ea1bcf0dca600117ebc14653b599151b614599054d6b82722 in C:\openjdk-8 
# Wed, 13 Jul 2022 14:51:18 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4c55ae81e7ef546e5541e735de9050cab9132f2d008845a8eea87f9cde19fd`  
		Last Modified: Wed, 20 Jul 2022 12:43:22 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a6041c25b88b4b2cb3c7930640de14826b020e4a8b156a74b5f63cae7bcf35`  
		Last Modified: Wed, 20 Jul 2022 12:43:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c302fef1d6a9df2c0413e5a4f4932d722c85e9ab6712f39a9bb2344b1739663`  
		Last Modified: Wed, 20 Jul 2022 12:43:20 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d6610344eeaa3c0e2b05b833b8cbe2543ae63857379657d2539b059ac347dd`  
		Last Modified: Wed, 20 Jul 2022 12:43:20 GMT  
		Size: 68.5 KB (68544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674bf3f1d3b4ca1d3a5ca60fb95ed13916c7e3827ea2dd0d377656c12af356ef`  
		Last Modified: Wed, 20 Jul 2022 12:43:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734687ecff19b161d662b10524b131fbb95788f43fec739cf647dff76432afa9`  
		Last Modified: Wed, 20 Jul 2022 12:43:34 GMT  
		Size: 100.1 MB (100078245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66b9e0541cf462575295fa667ef83fc269a6ffcc11480245e7bd8254841886a`  
		Last Modified: Wed, 20 Jul 2022 12:43:20 GMT  
		Size: 81.6 KB (81640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
