## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:91b84c4bb7491c42f87fcd05fc42171c8b846a312a5f1d3ed8348308a061bde9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:7857e4532dc7632dce52100f8afb5060e4c6c9ecd1096d580c7861c1a01930f3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142438653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c43d9f9c76dea3b6fc68556247a1a047f790ee7a337b58313bf49f9cafe6b08`
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
# Wed, 13 Jul 2022 14:54:44 GMT
COPY dir:3ac3da968b0a55dd3b56d678ae78ff2fe7435f143b42a50fa75d097fd864892f in C:\openjdk-8 
# Wed, 13 Jul 2022 14:54:54 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:8dd4c0628d8764fa48ba19ab6e6b4aa98dc599881e5aaa55014f4dc65fba407d`  
		Last Modified: Wed, 20 Jul 2022 12:44:36 GMT  
		Size: 39.1 MB (39129063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d71ca5c1d6875a7fb32458d7252f62a5676e3c2f9ff284f4e97f21cf252aa9f`  
		Last Modified: Wed, 20 Jul 2022 12:44:28 GMT  
		Size: 80.3 KB (80331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
