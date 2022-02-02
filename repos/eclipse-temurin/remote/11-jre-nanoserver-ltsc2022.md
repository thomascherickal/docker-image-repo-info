## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:fe908df968dab97488c5d11bac09bddd1f213141cb9af2b18fab835543e71408
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:74373f507c5612aa22248b33d046fd95a2da3b95aea448eccfb0f7444ed6c199
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.2 MB (160233211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:467e0034bec1f4bd6dfc993452605028f6e461cc94785bb477f12d0874092cd1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:52:20 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Tue, 01 Feb 2022 22:52:21 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 01 Feb 2022 22:52:22 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:52:36 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:52:37 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:53:45 GMT
COPY dir:37611e99da55cacf359232de16544a31f88bdb2203ee3a1dce3c1fdbd34bf2dc in C:\openjdk-11 
# Tue, 01 Feb 2022 22:53:59 GMT
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
	-	`sha256:10fe196388e251cce49885dcff2977445c7baba0c3dcc11c62e9ed2aebc7b555`  
		Last Modified: Wed, 02 Feb 2022 00:56:43 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2b17c070057bcb5870d992810f1c77c20c7ac765870e23a99eff8ac660d7a4`  
		Last Modified: Wed, 02 Feb 2022 00:56:43 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79b4c6f4858453b847c0947c691cf33544e764f6c134f06c911cf847c964a7`  
		Last Modified: Wed, 02 Feb 2022 00:56:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a47ff23b99b9e4e47b0c90611e6537b607287b08a9c1092a62c0afc809a1e0`  
		Last Modified: Wed, 02 Feb 2022 00:56:41 GMT  
		Size: 76.8 KB (76781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420d0c3862102a0f5e0b7c2750e4d050b52b79ddc791c2087575308e04a731`  
		Last Modified: Wed, 02 Feb 2022 00:56:41 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39dbfbd555a762bd1b034cdf6e61bf279ca4509965942a286eac3101c93cde2`  
		Last Modified: Wed, 02 Feb 2022 00:57:22 GMT  
		Size: 42.8 MB (42756594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06263ebe5e87a382d43015183b74bb98fed70dbf79d85c044197ec23c8f9cbfb`  
		Last Modified: Wed, 02 Feb 2022 00:57:14 GMT  
		Size: 60.9 KB (60926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
