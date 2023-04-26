## `eclipse-temurin:20-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:e2275bce5780eec09d2f0f7acd178441767c926367265ee8729524bed612764f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:20-jre-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:befd50a23d9c783df81bf5f3d8177d70b2c2da1e12cfd9bc3bacdc987ab73aea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155764068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf3057e1f334b58ce24ff8c5e30f9f61401020a3647a0e58260e7abc9a234fd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 26 Apr 2023 19:51:59 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Wed, 26 Apr 2023 19:52:10 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:29e70bcac2519026377a75e57519e15456cd994aa71702aad532359d603f5e41`  
		Last Modified: Wed, 26 Apr 2023 20:09:27 GMT  
		Size: 45.8 MB (45767285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc29a9850fbc1f1614abfa14266e852431085c860e545da806a280b36b3040`  
		Last Modified: Wed, 26 Apr 2023 20:09:19 GMT  
		Size: 3.1 MB (3134488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
