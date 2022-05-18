## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:6fe52de64c57ea26ccb6c800f1d2493b645709fbb27a994dbd4caf7b8e0039a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:1404f893d3c5d79eaae5a0b737646ab579f2de6c6b79be5fbed15de6484647ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (303046189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceac81698b5e05ddd9c975f7a046bf094f20758f079278cd701ebc01d826f78c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:24:58 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 11 May 2022 15:24:59 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 May 2022 15:24:59 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:25:10 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:25:10 GMT
USER ContainerUser
# Wed, 11 May 2022 15:25:25 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 11 May 2022 15:25:43 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:25:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f390bba55809b874fe5f57ce3a5a999a374ebd6210cbe044ae9d7eaa3eb9399d`  
		Last Modified: Wed, 18 May 2022 13:49:45 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133c9dd33e6a08c14fcf0aeacac91f0f5afb69f40ae80ceb172be1d62470c9ad`  
		Last Modified: Wed, 18 May 2022 13:49:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c982ffd7e946d7e9812b21bb8ac710ed07a2d6be5fe104c5642f758b7b3df958`  
		Last Modified: Wed, 18 May 2022 13:49:45 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4635a552a798a7a41cc2aea46ced5a20b73e2dda81269214dde48a3ac9b57`  
		Last Modified: Wed, 18 May 2022 13:49:44 GMT  
		Size: 82.7 KB (82682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666bc2ddefd40e6b032ee9e0ebb9529630b75e6951964aa480663c1d56e479c0`  
		Last Modified: Wed, 18 May 2022 13:49:43 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e43023105a800a7a722a6ba8c468618beff79e27f8d792a0fab72b6e5547e99`  
		Last Modified: Wed, 18 May 2022 13:52:54 GMT  
		Size: 185.2 MB (185207712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b355ba87b679906ace8610f2c7379d2b6064561560b4331f337c5e68faf2315d`  
		Last Modified: Wed, 18 May 2022 13:49:43 GMT  
		Size: 62.0 KB (61953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb44494b72ccc42d2b4b1ebd0ad1dfbefd763401ed638187c4c79804891660f`  
		Last Modified: Wed, 18 May 2022 13:49:43 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:0d11e590713961381f7092387ec98aa81369f69117c3077f7c633b0d13c43de9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.1 MB (292062079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8cffdd19a44e44a244a9cf29d9393c5b988819a451d6b5f6739b26e286cfe3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:07:30 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 11 May 2022 15:07:31 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 May 2022 15:07:32 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:07:41 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:07:42 GMT
USER ContainerUser
# Wed, 11 May 2022 15:07:58 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 11 May 2022 15:08:24 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:08:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8743647b8ae81c92754d445c24fcc8939c32453feaafa85fefb9b276cab329cc`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bab84fbf268fee41493c0a1d9cf46b40b6d040166aba8958fbc2c361b4f466`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c28f4021ca921cb65e2fe828836e1a891b3269a35543193d4c8f1932c94cf5`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4675ebe79379c89ba27a3579f9aef7ce52b76bad0e4978160afc55ee6573a6d7`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 70.2 KB (70154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1be201dab22ad99a45344d8dd0c83a049ac7f66c67ee69d254e23f83444cd1`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526981b83c5987ee605ff2fee424bd116f427296e9d92fbd219b918f3abbd22`  
		Last Modified: Wed, 18 May 2022 13:25:02 GMT  
		Size: 185.2 MB (185189434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fb8535124aead58723fae0c475eca7324aae8697da99a49c92a4561cdd122`  
		Last Modified: Wed, 18 May 2022 13:21:44 GMT  
		Size: 3.7 MB (3661732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fa3f936e0678af6ce3e38ed6e89f311708e27277749c0fe7e2ac014295785`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
