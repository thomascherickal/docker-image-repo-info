## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:4fc3e8d833642aa06df8df3a8a43099d585009261feac362385ecb4149afb9f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:f8ed9a48941a59d4fc28750692d105e2cdea5af3755b5d4802a89474bd079354
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141125459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a6ae749b827830e88e3324be3190eee28593d215c0b37d4808d0fe3c9d5952`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 17:32:15 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 25 Aug 2021 17:32:16 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 17:32:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 25 Aug 2021 17:32:25 GMT
USER ContainerUser
# Wed, 25 Aug 2021 17:32:25 GMT
ENV JAVA_VERSION=8u302
# Wed, 25 Aug 2021 17:35:28 GMT
COPY dir:58006f68c4ea109e560c76de14918bddd55bac9724011203b6cdeb031fa20971 in C:\openjdk-8 
# Wed, 25 Aug 2021 17:35:40 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d60db2af34dfc263a6bd1beec4934d22397163f3631bf7dbd1ddc4a0fb6cb`  
		Last Modified: Thu, 26 Aug 2021 00:50:22 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e764fa0c7e7599b95040da290d3db940fe5cc24313bc15bc3c76ff9fa2918816`  
		Last Modified: Thu, 26 Aug 2021 00:50:21 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d0d36c8cc2449af05f6ef9fff4d2dabd8f027fa226d1357c83b9a192a92fe`  
		Last Modified: Thu, 26 Aug 2021 00:50:19 GMT  
		Size: 68.0 KB (68009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746d6765bc24be916f6090b88bb3e999ca39f01f8f4bfec395d8ff85f8e67d4`  
		Last Modified: Thu, 26 Aug 2021 00:50:19 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7f2d29cd5ac0e8dbae3bb36f5a1a60a568dfe07d880dd776d53b586188a49a`  
		Last Modified: Thu, 26 Aug 2021 00:50:19 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd3ade84c43bae651177576c1c01c7d8ea4bce17380457597a7d653ec99569`  
		Last Modified: Thu, 26 Aug 2021 00:52:05 GMT  
		Size: 38.2 MB (38230828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71153ce4fc337e2d63a6e6f5f275fb24be3b443abfc33caacecc48794826f7fd`  
		Last Modified: Thu, 26 Aug 2021 00:51:24 GMT  
		Size: 80.2 KB (80235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
