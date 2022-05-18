## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:68094b2875958f720f08a3cefa1f644e022afdee3cebce8a5814dd8bdee6c2c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:60294dc92d546567ef9e06ac127d7c15d15bc25f715b35a2a00471ad0357789f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160964128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd61ec1b8a420c1d8526ed72edb0c299b896051d67b368f92d6dfafc4b532791`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 11 May 2022 15:25:58 GMT
COPY dir:c21630f3252a44226ea19120d87b000e49aedb9d546bbac0f6424fd80f37c64d in C:\openjdk-17 
# Wed, 11 May 2022 15:26:19 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:444019db2fdf00b91978570472e5aef562d70dd9a108467f35b3db05b79f322c`  
		Last Modified: Wed, 18 May 2022 13:53:53 GMT  
		Size: 43.1 MB (43126924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eace5f70d41f9b80cd1716c7c83f5404ea1066b51f9362d01d96df798283de2`  
		Last Modified: Wed, 18 May 2022 13:53:08 GMT  
		Size: 61.8 KB (61840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
