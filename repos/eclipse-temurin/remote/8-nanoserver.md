## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a1f1bbd1c01725a08973d94895ec42b412051d62fb3370c97c64ae1a5e687865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:13156820c0a6994ab799c893ac8d2787e2582146d22dc516c766ca3a7edcf2b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221584897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6be81b98b9d4fd0767840c96a71ee85fbb0f493d2b7143047ec39784985448`
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
# Wed, 10 May 2023 01:14:23 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 10 May 2023 01:14:36 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:ff3e923ed73cd1fd7eb746c2d28d2e02c489a1559145a3e22d03ce1e0e9d0e61`  
		Last Modified: Wed, 10 May 2023 07:04:18 GMT  
		Size: 101.4 MB (101444499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc31baf486e52d47ae75f3d9ffbebcae166cda39245a998383b7e9666745871`  
		Last Modified: Wed, 10 May 2023 07:04:07 GMT  
		Size: 59.6 KB (59606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull eclipse-temurin@sha256:84c9c3c55cab2ba124ae910328e0a5e315af68636728b9cabfd2563458dd9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205976995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d05ad18ec26aa4e4e4220d8ada8bb51418718135630c311cfdc8b2f7f1b20c0`
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
# Wed, 10 May 2023 00:40:28 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 10 May 2023 00:40:41 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:312eeccf4841bb89b4a45c82e39f10cb90184200e1569e36c923248e8569970f`  
		Last Modified: Wed, 10 May 2023 06:55:28 GMT  
		Size: 101.4 MB (101437506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0300c3b1414fd3a5a9898b6019dc8270a7354e0b3c623f3ba78eb6ec60cee0f`  
		Last Modified: Wed, 10 May 2023 06:55:18 GMT  
		Size: 85.1 KB (85103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
