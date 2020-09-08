## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:01056bd60dbb83cbc68b72193cd25ad17780794e60e85b558f9d75104bd1fbc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:250a8117bafb4335b0b114a955bb8524b6422f3f588d52604f28499c14016e99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138811133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f8ae7109380d20611457e36c16b62a247e1656c6f5c12f376690ee23d4d5c4`
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
# Tue, 08 Sep 2020 22:24:25 GMT
COPY dir:f9cdcac6b6965117d0bbadf86b5d0b55237954c067839a8e6ad0130705a48c8f in C:\openjdk-8 
# Tue, 08 Sep 2020 22:24:40 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
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
	-	`sha256:857b016c6d25bb25a7c0f763e751573d5defa1ae2e57e27aff66676a0d56ea48`  
		Last Modified: Tue, 08 Sep 2020 22:45:21 GMT  
		Size: 37.4 MB (37426058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64492b4c2f35f5086ef98d863ae2dde4c06e84eb915d605469f206e353ae7d6d`  
		Last Modified: Tue, 08 Sep 2020 22:45:15 GMT  
		Size: 77.3 KB (77346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
