## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:87aaa95cd659808474001cbfafbe1efad8c5a395423b3d043da6789662cb4411
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:cac14073bd5a70333043c35a1b5f422d35f60db96a14f33d0d4f64c08bbab204
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144512856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f683177ea21a171143e1446d78cc82169ebefe34be4a80ec7e45f0f23d6dace`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 00:41:51 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 00:41:52 GMT
ENV JAVA_HOME=C:\openjdk-8
# Sat, 24 Jun 2023 00:41:53 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 00:42:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 00:42:05 GMT
USER ContainerUser
# Sat, 24 Jun 2023 00:45:16 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Sat, 24 Jun 2023 00:45:27 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:f8b8d173676a3bebe8b880a2e576e384ab320c958eaa8545385db0739f0cedb2`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce8525b41ee8db302be09889fee5ba69376f2c6519486b55c8cb1256038610`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582c8ef87488af5189acceabd7a9e4f612a5facbf7909a977059bc8f4cbdd1d7`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71b624ae67158c8af0256f60f5a37249035a4067bcee97ba9a4758e65f608e`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 70.4 KB (70434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c1cdb7974f0d93a444a7f16f91f3ee0ee5a4766f1781f86e73a91e6ac74aab`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b802664ec6d61a0b46ab3287b65c25008db51c2cc57b7ed911cde6536a1ad82`  
		Last Modified: Sat, 24 Jun 2023 01:25:56 GMT  
		Size: 40.0 MB (39952084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4805cbbaf86e87d1560e811c8ee4d4130c323c576a38a1db1f581e4e5901`  
		Last Modified: Sat, 24 Jun 2023 01:25:50 GMT  
		Size: 83.7 KB (83658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
