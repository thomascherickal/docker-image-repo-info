## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:17c181eebf6afb0d44d6799f535ccf1eb834142dc79b8cd2525f61c636ac65cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:1db800679c7814de34f90a09bed88724e45f33e3d2699818d943889e542e4c27
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142324337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02caa91620211fae9ce958202cacb9d6ee923c2f999e0debe818eefae4f1df2f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 21:56:20 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 21:56:20 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 08 Mar 2022 21:56:21 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Mar 2022 21:56:22 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 21:56:37 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 21:56:38 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:00:56 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Tue, 08 Mar 2022 22:01:10 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e0065cd23a657c8f30ae5af121fd18451d2307835a1124ea57c80683eda26c94`  
		Last Modified: Tue, 08 Mar 2022 22:37:21 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a710cd9d2482732161f43d2683aebb5a1c4e62c2d3504b8accb12ea323bd78f`  
		Last Modified: Tue, 08 Mar 2022 22:37:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c8ccd0701d2cba8034e20b7dc639ef976375fca431231c953604b0454dd73f`  
		Last Modified: Tue, 08 Mar 2022 22:37:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46242a55e957c0068ecc56dc7b69993461e15d23a468633abefaed8b6986df27`  
		Last Modified: Tue, 08 Mar 2022 22:37:18 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6d47cd2b715622722bb7959789d36c0af4b7afb18441b6bb48bdb6bfa924a1`  
		Last Modified: Tue, 08 Mar 2022 22:37:17 GMT  
		Size: 69.6 KB (69588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed13388e71bf626ec62b079d5acf480de920c2612df2f786381c617509dd787a`  
		Last Modified: Tue, 08 Mar 2022 22:37:18 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0dfa3fdac5294bde5604bd644ace90ee9aa5467bac0e5c4cfafc7430a2182f`  
		Last Modified: Tue, 08 Mar 2022 22:40:24 GMT  
		Size: 39.1 MB (39112565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94069757d0687813639a9bc8fb1d044fb80cddf2aec97e3ff501b7debf37abc5`  
		Last Modified: Tue, 08 Mar 2022 22:39:40 GMT  
		Size: 81.9 KB (81869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
