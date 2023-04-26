## `eclipse-temurin:20-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:45acef55a59927595d3072a1df2e6d750d93b9f6720866c2b74e58f552f38210
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:20-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:556a53d4a4fc6352395ebd333a065f1f96f25e31cc9fc8a6428cd5a544553da9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.9 MB (305908204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c674947c74301dce89b41cdd6337b31d6bf846354b88b7d1ca9b79620c57d717`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:47:24 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 26 Apr 2023 19:47:24 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 26 Apr 2023 19:47:25 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:47:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:47:33 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:47:49 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 26 Apr 2023 19:48:00 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:48:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9598bb20f27c6107bfb9b3c52456dddb0f15922c42a75c0dccb0ccb07faf8de9`  
		Last Modified: Wed, 26 Apr 2023 20:08:09 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f894d926d1e9619f806c67d3a2213ebd4b26b5861e4e469c183c37d77cf9f26e`  
		Last Modified: Wed, 26 Apr 2023 20:08:10 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0077df2009cc07e2ff503a3928c6d29586c12e457afcb7e02cde9fabe46bac0f`  
		Last Modified: Wed, 26 Apr 2023 20:08:09 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a17cbb2fad43250ceb17c9285531a86e9b39bbcf7f509bd2c3badae36182425`  
		Last Modified: Wed, 26 Apr 2023 20:08:08 GMT  
		Size: 68.0 KB (68002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d1568c2dbe1e010c675971f32bdf9d8fa6b962f4afefa63a90751da6297a4e`  
		Last Modified: Wed, 26 Apr 2023 20:08:07 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d11b5b922d806215979b62bdefadebcf09967526ccbc10bdb50ffea01e1f7a9`  
		Last Modified: Wed, 26 Apr 2023 20:08:26 GMT  
		Size: 195.3 MB (195277063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662adfff9e36204c2c66e286f56c3330a7ce6dc008b163d144c5a351beff94c`  
		Last Modified: Wed, 26 Apr 2023 20:08:09 GMT  
		Size: 3.8 MB (3767818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bdf63f036c4b3f4aae772cec9a3a0958a8539c03de32c38f0d3b34ff67b667`  
		Last Modified: Wed, 26 Apr 2023 20:08:07 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
