## `openjdk:8u332-jre-nanoserver`

```console
$ docker pull openjdk@sha256:ce33e715aedb08e8ba5e12d4bf793e628a6efbe0d2bc28478504727b960b6a41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:8u332-jre-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:75d784068022c3f98ca27291035c5253189b3806051167e9f568c4ec9802d2a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141552497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd3d1cb045deb0f866afdad6975f60308cb767f73f944bf1c6dfce9f0aa82b2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:50:29 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 15:50:30 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:50:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:50:41 GMT
USER ContainerUser
# Wed, 11 May 2022 15:50:42 GMT
ENV JAVA_VERSION=8u332
# Wed, 11 May 2022 15:53:18 GMT
COPY dir:a69662fb25cadf36484d90c7c9990719015f86fa8a02dabf235af3b8f20f255b in C:\openjdk-8 
# Wed, 11 May 2022 15:53:32 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e686895fdd8f684d42cd3b3cb6b3d81d8fcf7476edc963ecd72ee11da2ba562`  
		Last Modified: Wed, 11 May 2022 16:24:33 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37520d359d3aef49fdbd396ebf8a57a65f3d2caba5069c46f2cf3c931aa973f9`  
		Last Modified: Wed, 11 May 2022 16:24:33 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0d64670d05bc44f4ea58aa4810dfbf3eca978ba978d17932ff782ad916beab`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 74.8 KB (74840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74363e36ea7d830221ad4ca73ea1a764a3e23479fa83cf3cc6c7a2df09513b43`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb4697c0acf8cb41498969c7aac9177ed4bf280de0caf1a5e7a108face8349`  
		Last Modified: Wed, 11 May 2022 16:24:31 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d99f853331ec0645799521bbe51e75195f779f3930bd0d24837d2e7a2e9e479`  
		Last Modified: Wed, 11 May 2022 16:26:47 GMT  
		Size: 38.3 MB (38288198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0bfb0dc615fb0d69620bd966d34fb2dd98f5a953d295002b8f9ab258eeb94e`  
		Last Modified: Wed, 11 May 2022 16:26:40 GMT  
		Size: 49.8 KB (49804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
