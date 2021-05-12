## `openjdk:17-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:8254ac10031b59f15300e57df64befb05b163af6f88e5801150e8c5549ef14f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:17-ea-jdk-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:129774a096b38aba672d28c8a1338d847d9844b4c61f467864e4790fe46ac77c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286090242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eced16a66e7de12b0ca297f5df2d09b8637afbb038f25f9fe5167cd4354d9af`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 16:42:56 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:42:57 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 16:43:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 16:43:21 GMT
USER ContainerUser
# Wed, 12 May 2021 16:43:22 GMT
ENV JAVA_VERSION=17-ea+21
# Wed, 12 May 2021 16:43:40 GMT
COPY dir:cfac9f56777a5d91e0879764fa534bb67fcf5d706baf09e8f4a88eedb9974a0b in C:\openjdk-17 
# Wed, 12 May 2021 16:44:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 12 May 2021 16:44:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea91a7775c05d55a850a2983043468ce6ded7406743836cf8f33afb037aba1a8`  
		Last Modified: Wed, 12 May 2021 17:16:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0a5b4dd190af3527c02bb783babc5d88014a4de37555355c2f7a59dd21449`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab5fc14de7c93823ea1579b64e1e79017e9738a39e5d165aeed23c15bf7ffd`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954cb2ae96dfb0f537ce02738b91077c41cda7743ff097b99d8a6cfc74e211f`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 69.5 KB (69533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95581d66523cc5b44afdfbd1f1e7732689ad5d73bf1c1352ef8f1e669dceede2`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62976dd7fdadb1b22bdb1588266dd641152764a88529bb988f18306320f7ed8a`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633ccac0e2d7e3dfa3e8e967e2f28b9239530eb67830a23153d539e605ffe93c`  
		Last Modified: Wed, 12 May 2021 17:20:32 GMT  
		Size: 181.0 MB (180986869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13dc2b5653af304c87daa628568e47039a08c3098248da35aa98bd8db85f9ba`  
		Last Modified: Wed, 12 May 2021 17:16:38 GMT  
		Size: 3.7 MB (3651706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb857706b0a7e7d93ad6be98f89d8ef2fc632133b0af3100dc92ef46ea86fd7`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
