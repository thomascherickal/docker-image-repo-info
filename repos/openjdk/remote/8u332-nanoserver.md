## `openjdk:8u332-nanoserver`

```console
$ docker pull openjdk@sha256:09ea6f9d4ac9a02716e411e7a21e07708149bcea9f87b377a4a5ad3322100da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:8u332-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:3135609dea3b842f8eb294d39d5b5775c1352e0c1a295b015619138804d58cf1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204236420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a799074d0565568a3ff8781e27b3c75aa8b0de28a5c09663c1285615de6d996`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:50:29 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 15:50:30 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:50:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:50:41 GMT
USER ContainerUser
# Wed, 11 May 2022 15:50:42 GMT
ENV JAVA_VERSION=8u332
# Wed, 11 May 2022 15:50:57 GMT
COPY dir:679ecdc3b1aa3045788b8b611f7a86f57009d803f478419678a6098b0a258b48 in C:\openjdk-8 
# Wed, 11 May 2022 15:51:10 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e686895fdd8f684d42cd3b3cb6b3d81d8fcf7476edc963ecd72ee11da2ba562`  
		Last Modified: Wed, 11 May 2022 16:24:33 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37520d359d3aef49fdbd396ebf8a57a65f3d2caba5069c46f2cf3c931aa973f9`  
		Last Modified: Wed, 11 May 2022 16:24:33 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0d64670d05bc44f4ea58aa4810dfbf3eca978ba978d17932ff782ad916beab`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 74.8 KB (74840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74363e36ea7d830221ad4ca73ea1a764a3e23479fa83cf3cc6c7a2df09513b43`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb4697c0acf8cb41498969c7aac9177ed4bf280de0caf1a5e7a108face8349`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4721e7da60400824a7238d9f4b9aa77fa6c0e42a17f1a4610e8282956eae1a`  
		Last Modified: Wed, 11 May 2022 16:24:44 GMT  
		Size: 101.0 MB (100971045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323dd53e6af8fcdd5eed7c7dd523661f60b6a7fc60653fd016ec3c30a5efbb83`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 50.9 KB (50880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
