## `openjdk:8u332-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:f71fdabc06e816bf7d0900a2b3c78de6d6804fea0dd672176050781fc46a77dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:8u332-jdk-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:ae0b9098dbefcc56a133e5aaa32dd9c58e396750608df4188a1184a80455fe97
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204212049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a429412809a2656869aa92aa8a5af06482e938886924120738d7ad05cab9b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:21:37 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Apr 2022 17:21:37 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:21:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:21:44 GMT
USER ContainerUser
# Wed, 27 Apr 2022 22:19:38 GMT
ENV JAVA_VERSION=8u332
# Wed, 27 Apr 2022 22:19:53 GMT
COPY dir:679ecdc3b1aa3045788b8b611f7a86f57009d803f478419678a6098b0a258b48 in C:\openjdk-8 
# Wed, 27 Apr 2022 22:20:06 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65fb95ee42514e5278fb1f68d4225d0a5bba71921defb635d841ca30789226f`  
		Last Modified: Tue, 19 Apr 2022 01:19:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b00dbd36f2154a4eabea44e9a5d88c98927e03b469bb16de373838d0f29d1e`  
		Last Modified: Tue, 19 Apr 2022 01:19:34 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c635236ace6c57e8af5a6a467722bb1484d5ae5aaf133d60a5475aef5f4d2c4`  
		Last Modified: Tue, 19 Apr 2022 01:19:32 GMT  
		Size: 72.2 KB (72156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9131ef298cbc9163210fbeb93d70aed6922673cebc88b8563ea8ea489357b1c`  
		Last Modified: Tue, 19 Apr 2022 01:19:32 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916d4a5c260a30f1a16a40718d959ff928c900be9607f848103cd78e06b236`  
		Last Modified: Wed, 27 Apr 2022 22:28:39 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80ab14ad4194e22c7f09792b191567ad0df946be70b66d7faee93f1224861d1`  
		Last Modified: Wed, 27 Apr 2022 22:30:25 GMT  
		Size: 101.0 MB (100951921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35cbd6739b1b921278075c90a72d0c38198d01fdaf9f7a767b415231a2edae5`  
		Last Modified: Wed, 27 Apr 2022 22:28:39 GMT  
		Size: 86.2 KB (86177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
