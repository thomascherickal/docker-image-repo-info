## `eclipse-temurin:8u372-b07-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:daa47f2bb4b7262e08ba105c9cc2b5772b05e9eb1e61a178bb6b17ddb63c7f2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8u372-b07-jdk-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:4f209ca56b2404a64040d5bab8c04dc5b68991b71d7e34b90c5caba39a9719b2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206006886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc832ae38eca57d2f8e2e4eb53da552fd22c8a3d990c1d0906ce6ac749968674`
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
# Sat, 24 Jun 2023 00:42:18 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Sat, 24 Jun 2023 00:42:32 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:8ccb2b2e72a38e5ffb1f29246a8936ef276a1dc3a2d028fdaea78449a21b1b24`  
		Last Modified: Sat, 24 Jun 2023 01:24:54 GMT  
		Size: 101.4 MB (101446981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91894ebff21232e2e38ba57556b29da5eac4589e2fd7b811f1dd55c39266245d`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 82.8 KB (82791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
