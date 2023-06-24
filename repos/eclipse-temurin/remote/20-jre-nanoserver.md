## `eclipse-temurin:20-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:e9af5a1afd122438074654c39cbe092c3aa5eb1fed374aa5a3b3187237ddb2ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jre-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:7fc3c537564eff3cea58d1902da95ee4333901e93020fd5897b51bd07158d044
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165933020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4561adf66f3709c59ee8b1bbbf27a4a4329dcd708b65de74054c5d8cc452ac56`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:12:24 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:12:25 GMT
ENV JAVA_HOME=C:\openjdk-20
# Sat, 24 Jun 2023 01:12:26 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:12:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:12:36 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:13:24 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Sat, 24 Jun 2023 01:13:38 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81a88fd1e4270664dec2ec13169bd88eaa6b8b019c0fb48e06635378a709617`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c800fc714f89a75e5414a4597fac693e9d62be65fbd8c222f44cda41f44bc3`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfabed7da3438545b6544d6e2199c88812bd45e313099b56799677cbdc6662d`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81fe92368b73ce26b0fdba745b718c2f43c9c41458f9e7e0a7322ee849e7e0`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 80.7 KB (80715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f4a0aeb9583372b005ddce4994d5e31d4073d82f3d3fc4dd8d7efa1238aef9`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d9caedc8c1342cae7cfc87ab575e5b7cc64b8f1a943d0e475229e3990a6e7d`  
		Last Modified: Sat, 24 Jun 2023 01:37:26 GMT  
		Size: 45.8 MB (45757473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d443337d9ac727b245f3d032f42e5578d129d06e963b5b75dfccb9bde98f43d2`  
		Last Modified: Sat, 24 Jun 2023 01:37:17 GMT  
		Size: 60.8 KB (60794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:744642b418b091668f5acbc461d4d18176de6b848401fd3000f734346dd7c420
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153378967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1557e8933f7706a69b7dff1f5397677050fb2a4bd50b17eec8bcaf99aa6cb65b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:04:02 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:04:03 GMT
ENV JAVA_HOME=C:\openjdk-20
# Sat, 24 Jun 2023 01:04:04 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:04:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:04:14 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:07:45 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Sat, 24 Jun 2023 01:07:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:09087aac643f57e5e24f95fe0a1c8519d0f93dfcf4500263516c0f3874290109`  
		Last Modified: Fri, 23 Jun 2023 02:23:11 GMT  
		Size: 104.4 MB (104400893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09be2e47b3dff420361e93d34eaadedcfd9549c9be5bd77936370792babf874`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f867d2c4f284f34f17dbc421aadc9e0fbec404d33de133b85670db5211e77528`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299bed8971d729fd6ea364dd0fdea58af4cbed817932cdeadb0e2ce5280817f`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef55d7fc9b89fa790f54f2685e2644e68328f51c1bc1df43d652db4d15b32df`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae46e058dfc9dbf46033443d916af0a2155c758187110e18f5da39d047ef69`  
		Last Modified: Sat, 24 Jun 2023 01:32:52 GMT  
		Size: 69.5 KB (69460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5713507914a5a9e5750810b925cdffc1f0cb3a926b162f73e1360e13b4c7c1`  
		Last Modified: Sat, 24 Jun 2023 01:32:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b135220d5e222121d799f784dd785980d9d8d0e12926260f4baf9645e5dbe5`  
		Last Modified: Sat, 24 Jun 2023 01:34:11 GMT  
		Size: 45.8 MB (45767617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df7f8cb8e34e341de84e82335cbc4eb53ffb6a2c53c1f92ff5e688113a41638`  
		Last Modified: Sat, 24 Jun 2023 01:34:03 GMT  
		Size: 3.1 MB (3135129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
