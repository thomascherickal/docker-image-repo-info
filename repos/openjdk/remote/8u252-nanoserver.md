## `openjdk:8u252-nanoserver`

```console
$ docker pull openjdk@sha256:4778d157dafac76c9a6a5c76aec17aec802a1a8dfb5d0f4ab8ebcbdf9f1e8e20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:8u252-nanoserver` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:4a539744ac2bf01b52d64aa40af9bce6c79b293cc048da550d2c61d6a2401239
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200894911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e135d67b8cb8f35d22dadffb7a61a1e17cd0388228f789b8caaf33bfb9929d42`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 15:30:41 GMT
SHELL [cmd /s /c]
# Wed, 13 May 2020 15:57:11 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 May 2020 15:57:12 GMT
USER ContainerAdministrator
# Wed, 13 May 2020 15:57:23 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 May 2020 15:57:24 GMT
USER ContainerUser
# Wed, 13 May 2020 15:57:25 GMT
ENV JAVA_VERSION=8u252
# Wed, 13 May 2020 15:57:58 GMT
COPY dir:ab479e12b22d2d8e4d7a7f2a7c1ce2c9a985b2211941ab66c77b1be78e3ec440 in C:\openjdk-8 
# Wed, 13 May 2020 15:58:16 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c597e8fceaeb76628095f6dcfa538d497e85739068a817b45d73be2b96a3b37`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab776ab4b50d0cfd71683078381ed7262c0714503d1c51a1c1a17638582efb1`  
		Last Modified: Wed, 13 May 2020 16:29:15 GMT  
		Size: 824.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95de4896b5ed497cac9ccbb2ed31616aeade69a3c79b64b15196f19097b31500`  
		Last Modified: Wed, 13 May 2020 16:29:15 GMT  
		Size: 815.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d09afecfcc0bad842ec8f2307cdb919b3340e6af09ec581d45fcfd9f60d99`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 71.2 KB (71155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb3c5b23798be09045e18678d06d3941c514f0737db5afebdc8e7da58d7d08c`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059a1563d2f1af8c439c8c7d613fdd205e7beba82ffc15ee22d2ae3c37012f9e`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46902d84250f6fed8b2deda1d04d545f13179306156a530503c75ab05a1f8974`  
		Last Modified: Wed, 13 May 2020 16:29:25 GMT  
		Size: 99.7 MB (99747000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb736a00f3483487c035516fc7159915dd8b3586e1b1bd542490f20e4c84d69`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 52.6 KB (52647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
