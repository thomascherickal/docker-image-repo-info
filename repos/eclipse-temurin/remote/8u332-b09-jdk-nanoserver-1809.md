## `eclipse-temurin:8u332-b09-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:0969a4c8c33caa8d463d55a8ff2682b2ccb71b99ba8e48711d78d00a5f98dec5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:8u332-b09-jdk-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:810d2b70b43f5b4fc7e85e33ec0a9890fa66c3194ad71394e2c1339db29ca732
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203381576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d398dd0a261183066851d681511910d8d52c25ef97d1a0f630734619585e5129`
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
# Wed, 11 May 2022 14:50:19 GMT
COPY dir:fe4a23cbc3aecb3ea1bcf0dca600117ebc14653b599151b614599054d6b82722 in C:\openjdk-8 
# Wed, 11 May 2022 14:50:43 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:7f9dd42065f0f04a0fed48f01db6e73874dce61c6471bf2643b2eaa72456e36f`  
		Last Modified: Wed, 18 May 2022 12:49:52 GMT  
		Size: 100.1 MB (100078208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640d6635e3924f07bb36ad9f72a1adbda37cbf51321088e20668f180a4e6bcd2`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 92.2 KB (92168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
