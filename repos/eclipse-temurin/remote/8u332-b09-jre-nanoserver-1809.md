## `eclipse-temurin:8u332-b09-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:281e53f8dc6d86090f44d4a63042a46655a51319a81f514d113f843b14cf9255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:8u332-b09-jre-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:7915c9683e8866d781eefe025b9ffc812dcd68af767a003ac14ff009ac8585b3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142430116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4d8d6dfa081ed0422ff2cca315d486c10abb9858fccea2470b3b49a4431535`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 14:49:50 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 14:49:55 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 14:49:56 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 14:50:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 14:50:08 GMT
USER ContainerUser
# Wed, 11 May 2022 14:54:14 GMT
COPY dir:3ac3da968b0a55dd3b56d678ae78ff2fe7435f143b42a50fa75d097fd864892f in C:\openjdk-8 
# Wed, 11 May 2022 14:54:25 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8f2d99fa851deac0639d979721826197aba4963756d87edeaf12032faedd61`  
		Last Modified: Wed, 18 May 2022 12:48:04 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3f910a21f3d10321cc1617d1b47c075fa7cec8b190d21a0f8807a4af23b1a3`  
		Last Modified: Wed, 18 May 2022 12:48:04 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6196adacbbe2e54691328cdb81fa066ff43b86a6845d03f35d6ef4aeb75f39e4`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc662c0e9d3403199980e18b76f971e116138abeab04d82a9c20c3e10cf141f6`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 71.6 KB (71624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104a305619c88b65c3abb22985c69844c5289590d3d6657759e618aa0d59427`  
		Last Modified: Wed, 18 May 2022 12:48:01 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35764a4aee192fd7b7f76838fe479363852aefe6c1d11d72941819bedf826257`  
		Last Modified: Wed, 18 May 2022 12:52:34 GMT  
		Size: 39.1 MB (39129684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89963d6b4f691e250e5bd69bbbfc8af8afedecb0f5e7ada8cdd77cea43c8126`  
		Last Modified: Wed, 18 May 2022 12:51:51 GMT  
		Size: 89.2 KB (89232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
