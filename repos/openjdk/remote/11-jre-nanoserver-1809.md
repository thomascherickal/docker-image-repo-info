## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f6985e175c9160baf434a0d41da1681cc3a5199a841d91524e730649a0f8c722
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:34b1f8099a7e5b4feb542f4bc7634c62ff1b5905e3513f830c63e163d7ec2090
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140391659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0676ec2cbe246c23ee09ea991d0f820ee5752f1d4ce809bd2c8b7ea95dc1bb1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Tue, 14 Apr 2020 21:42:38 GMT
SHELL [cmd /s /c]
# Tue, 14 Apr 2020 21:58:31 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 14 Apr 2020 21:58:31 GMT
USER ContainerAdministrator
# Tue, 14 Apr 2020 21:58:42 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 14 Apr 2020 21:58:43 GMT
USER ContainerUser
# Thu, 16 Apr 2020 00:56:43 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 30 Apr 2020 19:15:39 GMT
COPY dir:5079dca1201fb18611f476ef87596f1f7b8bce8e365c08f25921689ee5b44ccb in C:\openjdk-11 
# Thu, 30 Apr 2020 19:15:59 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:895ca47ba9cf1a5b61a0721217cfcc038bbe9a4987c7536321c3ac51ef8e5e0c`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7bb74a827df2fe632673230eb22408cd5980851f1ccacda1fb1455b5b57b5f`  
		Last Modified: Tue, 14 Apr 2020 22:22:08 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37292e82c381bfd95f2c023e25d3128e79e30e4697e7d3060aef26e417a38f3`  
		Last Modified: Tue, 14 Apr 2020 22:22:08 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ebb398aa8f5bccb4e81fcb0932368a58fcfde4b33666e7468ef8a82e116a70`  
		Last Modified: Tue, 14 Apr 2020 22:22:08 GMT  
		Size: 65.4 KB (65430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891faa9eff3b21ae96bb207286120e1389355b2f057a63f73417fde08bab028a`  
		Last Modified: Tue, 14 Apr 2020 22:22:05 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a8ddcb1c304ac762e65372d1f672f8dfa722d64d0064bd47c6353c78af11b7`  
		Last Modified: Thu, 16 Apr 2020 01:12:10 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf236f5baa3a6327b32bb382a55dea9cdcf2ab7058a133a376d4f855e44023`  
		Last Modified: Thu, 30 Apr 2020 19:19:34 GMT  
		Size: 39.1 MB (39121145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae655794d09264420155b5f728407abf4cff0fa92f923f6336c7fb630c99a2c`  
		Last Modified: Thu, 30 Apr 2020 19:19:25 GMT  
		Size: 82.4 KB (82386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
