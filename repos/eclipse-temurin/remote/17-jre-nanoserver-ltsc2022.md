## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:6be847ae4101713fdb245c7a0bdaf3943af664853bb0b2e42aec3b52ab134820
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:3b648edcec4dbc9f22c98ff2227c3a8587a11033dcc0f253e73a6e1bee8fcf3b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160577739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561d87822dbfc01d1202323d0da28fa5749bb145b0a56a838ae174807c4b68bc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:43:57 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:43:58 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Jan 2022 19:43:59 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:44:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:44:14 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:45:22 GMT
COPY dir:38eebe4e3a4da98e178f49482de333d171d427f5886e68b2b67715641b9694d5 in C:\openjdk-17 
# Wed, 26 Jan 2022 19:45:35 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774536782c1c4d4015e8359ac0437fdb94a8d696f9cdef5e9936e721b99ae1f`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12214b1befa142979cea977dbe18e01fc824195c2dd83727fa5b15e41c38638c`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff8a2a945a4d41d4a21c3e74b99a007be23a149c47ec52f2f33ddf270bb6f16`  
		Last Modified: Wed, 26 Jan 2022 20:30:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ada735cfb773a4d0ed93bd8768bcc1e11e8f13d0f5e8ebd60b41a1cb4c9f8`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 84.6 KB (84623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf9b071a062772e3a9bd393d34c0fae1dd2444a5298988e86b1daa21b0f785c`  
		Last Modified: Wed, 26 Jan 2022 20:30:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2ac933ed9e13c571120b9d64174225b8fddc00d264c48a751ae8bb7f6870f8`  
		Last Modified: Wed, 26 Jan 2022 20:34:45 GMT  
		Size: 43.1 MB (43092394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05696213a4898846852c943181f4e0fd8d3d61bd912e2fe8f1de99b22111eb9`  
		Last Modified: Wed, 26 Jan 2022 20:33:54 GMT  
		Size: 61.8 KB (61799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
