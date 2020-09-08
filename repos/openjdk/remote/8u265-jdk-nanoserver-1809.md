## `openjdk:8u265-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:4341bbaa9cc68de1cfd186a3908bbbbd6b55d9a3015c7730b36ee89f66eaf1ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:8u265-jdk-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:9d5c56a7f6d5253b33fcc71df620bd62fa9ea9d7b5e70a6bcb9080bbffc44d76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201504853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaa504e36d4d8c6d41768cbe3d03597e404703ef8e8a8eb154d9891d96f5b43`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Tue, 08 Sep 2020 20:13:38 GMT
SHELL [cmd /s /c]
# Tue, 08 Sep 2020 21:19:47 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Sep 2020 21:19:47 GMT
USER ContainerAdministrator
# Tue, 08 Sep 2020 21:19:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 08 Sep 2020 21:19:58 GMT
USER ContainerUser
# Tue, 08 Sep 2020 21:19:59 GMT
ENV JAVA_VERSION=8u265
# Tue, 08 Sep 2020 21:20:26 GMT
COPY dir:3c2880b061bc00940ee162754a64e55567e0dbb10e65b749277b54fa005ce8de in C:\openjdk-8 
# Tue, 08 Sep 2020 21:20:44 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f72ec155bceaba8b4a5cdbd7aa79586c7296a801af5364a691c46191c910e2da`  
		Last Modified: Tue, 08 Sep 2020 22:29:01 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f76130165e8e081e20920b7cd0d2accf07f4413ef8729b5fd15552a9361551a`  
		Last Modified: Tue, 08 Sep 2020 22:43:39 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d562646dffac93403ed16e5c78c02679022f442b8c9b533032d245bacae89d`  
		Last Modified: Tue, 08 Sep 2020 22:43:38 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a631600b80813637faee63d4a91d54f54291f7479827c5dc927e43c1a5cbdb`  
		Last Modified: Tue, 08 Sep 2020 22:43:37 GMT  
		Size: 64.2 KB (64196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d775d3ed147970edf9c467e4795f7013daa842d1e5cf6292e5273149d11015d3`  
		Last Modified: Tue, 08 Sep 2020 22:43:36 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088e0370709ba80962bb82cb2424a3c1322d439921ac1bead98ebd5d1c6d895c`  
		Last Modified: Tue, 08 Sep 2020 22:43:36 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9573a2ae15bf4b6b5f070bbfefa613ffd507e21b387f23088fa2afbc96dece6`  
		Last Modified: Tue, 08 Sep 2020 22:44:23 GMT  
		Size: 100.1 MB (100111452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89aa6d5a0ebd35280c369bed93d898a8ca4192654a061bbcd45b6736c1cebb0`  
		Last Modified: Tue, 08 Sep 2020 22:43:36 GMT  
		Size: 85.7 KB (85672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
