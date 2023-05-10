## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:46b69f10734ea7ae48c9cf5e7fb235cd4d5f379376c90c56238575ba0e88aa51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:494407580e60472443371e87c877f5f2fbb160f6a0c6fdd4dd7066b115258db2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160098325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715241fe081cdf4d31fde58dd2f92721e6744a1fcff3dd588a645aeb4087a82d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 12:52:54 GMT
RUN Apply image 10.0.20348.1726
# Wed, 10 May 2023 01:13:54 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 01:13:55 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 10 May 2023 01:13:55 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 May 2023 01:13:56 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 01:14:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 01:14:11 GMT
USER ContainerUser
# Wed, 10 May 2023 01:14:51 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 10 May 2023 01:15:02 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:7d382efe6974b94c05000b6a95c1fd28e1b8bb3e81cc4592b2aa1cc46b90192c`  
		Last Modified: Wed, 10 May 2023 01:48:23 GMT  
		Size: 120.0 MB (120001338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cfc306feea2a215b4a83a66480231042a4bdc8001d07d634086f52f1f5ab3c`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094733d5dadab2bef8ab3368427e514ab7e30f25fd583e7f0b79e1211370a26`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412fddde1681c84b2b6a8927173afc2fe9f93af018bce16dc94aba6a8d607f90`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227787a081ea4e59e27ad44da06e67980f31d6d33f0ad0cde9d223b1922eab27`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefb1da43198006e4e845e7bf1fedc9f9ba423bf9b29f4e1ce47219bd03e2218`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 74.2 KB (74162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ecff3816dddd3fa41f2288c8e2d63096dd317b3032ff212861de09a424eadd`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699808bf398d6b75178eb7adbf93e390a88e77cfb76acbe29a56d4e6527f3808`  
		Last Modified: Wed, 10 May 2023 07:04:34 GMT  
		Size: 40.0 MB (39957886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdcf6c8f1f5b27eea70c4fc14804782ed62b55d56796fd8e59b71c099a8d4d2`  
		Last Modified: Wed, 10 May 2023 07:04:29 GMT  
		Size: 59.6 KB (59647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.4377; amd64

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
