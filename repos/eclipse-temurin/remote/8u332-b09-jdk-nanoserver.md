## `eclipse-temurin:8u332-b09-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:8256dd7fd8a418afd0ed3894a3dee078726752c7226d63180a61550e97188282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:8u332-b09-jdk-nanoserver` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:11ceaad0c39c7020033244de0b9d97722fabd62ceb3103f7af31c502fe79da53
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218260608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff8ea5fa7418d2bbe700510cb2244742c974c5eb00624162899aa9cf1f6caac`
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
# Wed, 13 Jul 2022 15:22:32 GMT
COPY dir:fe4a23cbc3aecb3ea1bcf0dca600117ebc14653b599151b614599054d6b82722 in C:\openjdk-8 
# Wed, 13 Jul 2022 15:22:46 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:49fcf698aee1c2e1a3f4b1cdb4eb048b1448dcc5ee8ffc055e825ca106903b2e`  
		Last Modified: Wed, 20 Jul 2022 12:54:24 GMT  
		Size: 100.1 MB (100071471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03335d65f5512be2176299e11d59ae23d7c6c5d64cc9d6f8dbbab15ff130d8d6`  
		Last Modified: Wed, 20 Jul 2022 12:54:10 GMT  
		Size: 61.0 KB (60959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u332-b09-jdk-nanoserver` - windows version 10.0.17763.3165; amd64

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
