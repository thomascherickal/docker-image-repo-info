## `eclipse-temurin:8u332-b09-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:0c70c6e681f6396f18b2026cb927046a224120dcca0e7c2ff8d0204bbac8518c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:8u332-b09-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

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
