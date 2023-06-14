## `eclipse-temurin:20-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7e7d90274b32a270b4e5175b28e1d916807ad332646c223f027cc35ad5075f71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jre-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:9d27e730abc5945e6e2ce911b5df4fd92c8a139d03c30e2a06f4e0ce3e14d154
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153338578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e4e36f35eb9e34a8d5fdc4a0a3cb09a5c537131073f667ff277e003a92c015`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 18:06:12 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 14 Jun 2023 18:06:13 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Jun 2023 18:06:14 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 18:06:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 18:06:26 GMT
USER ContainerUser
# Wed, 14 Jun 2023 18:09:55 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Wed, 14 Jun 2023 18:10:07 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5383d811aabbb2805907b3a15e1035fbe6d36d6ff2baced872afe06c93d85a57`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa085cac7c91c46669d4f8f81573dd462e288a713b4499ff83a1c7d1b46a58e`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfcac3d53075ad26971a6d98b48737f821c4cce49b09243478ccbb037692d4`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9503cf15848877aadb5fee8ed3896908826a4b1623697603a6c1d925f565ad02`  
		Last Modified: Wed, 14 Jun 2023 18:35:21 GMT  
		Size: 71.0 KB (71018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286588e2ded622d2806a7ee81d5dbfcfdfadfd2cb85980d16c15ead49ee8b0d5`  
		Last Modified: Wed, 14 Jun 2023 18:35:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5b33ca74d97d82f6d8ac33221053c930c530496b748a8706547a2d3ba74984`  
		Last Modified: Wed, 14 Jun 2023 18:36:42 GMT  
		Size: 45.8 MB (45755622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8d53ab45a69d9b57c6599725bb0d2d262bbf4e02375d06c71109d2177b79aa`  
		Last Modified: Wed, 14 Jun 2023 18:36:34 GMT  
		Size: 3.1 MB (3108254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
