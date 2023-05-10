## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:e67689f0d9b4ed4f5e2aae812ffa99196fed771a03efe5c6d095fd5d43f593a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull eclipse-temurin@sha256:7cd2053c8bde351dce4915a22804a8c1e9db81aa8bb6e7b48699abbda0311b58
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144486240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d998eecff97add04b883a1c4cc5bfa8fa037182085665b95744dcc4e76590d8c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 00:40:01 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 00:40:02 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 10 May 2023 00:40:02 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 May 2023 00:40:03 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 00:40:16 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 00:40:17 GMT
USER ContainerUser
# Wed, 10 May 2023 00:44:38 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 10 May 2023 00:44:48 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b79dd15c5dd82bc10521b9a4e49241f70088bc6edbb286f90be198abea55e23`  
		Last Modified: Wed, 10 May 2023 03:01:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428d16ff436c91c8dfb9565605afe75b42af2cadbd6e783e46f52b7e86a804ff`  
		Last Modified: Wed, 10 May 2023 06:55:20 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9569fa031b1fd4b38faa8730950239f045b9e3ef4b2f99f7e4ccb96fd3cf83`  
		Last Modified: Wed, 10 May 2023 06:55:20 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f647146e01827d82c277729ff10f65a76b6d1d70f00c977746cb09c02f180d4`  
		Last Modified: Wed, 10 May 2023 06:55:18 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6868e562259c3553e0dd3fb33b3d73fd6abbb9c98354b27bba53d950d64f740`  
		Last Modified: Wed, 10 May 2023 06:55:18 GMT  
		Size: 64.6 KB (64603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05edb7d77a9682750550109c8222e889f87160cfcd9b02fa476d92160884178`  
		Last Modified: Wed, 10 May 2023 06:55:18 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f51c7c4dc4b9a78bcd2fe77826761c6e4a90f29dc79f9689435755728b99f2e`  
		Last Modified: Wed, 10 May 2023 06:56:16 GMT  
		Size: 40.0 MB (39952982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebffc7276229433cc1b0a937e4265b48334365d10dc1b35446c439f8d270165`  
		Last Modified: Wed, 10 May 2023 06:56:10 GMT  
		Size: 78.9 KB (78872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
