## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:2de7f9040c25402ce798540863283ce3ebaa527d8f3fd0b991292c7bb7e975bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:284bbf5c43738b3d375f5f382ad1f606ba9559fe16303fed4caa7000e5803e72
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.8 MB (156761516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6736cf2c4059ec77119c71361a763b8fe093d2c666cc31a54b59af6147ba18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 04:50:34 GMT
RUN Apply image ltsc2022-amd64
# Tue, 08 Mar 2022 22:26:00 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:26:01 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 08 Mar 2022 22:26:02 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Mar 2022 22:26:03 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:26:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:26:22 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:27:06 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Tue, 08 Mar 2022 22:27:21 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:dad81795ce109a7e20ebf80ad31925797ed97f9ba2a559f13f96ce3be5ea712b`  
		Size: 117.5 MB (117485491 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ad17ae3a2fc5cdf554f0d828bd6d04e79f37ae3dd800a44c8a3a1892a57b75c3`  
		Last Modified: Tue, 08 Mar 2022 22:57:38 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4749e2ec828a56fc6fc213ac46fa35a61ead2426dff1a91b404f563f30d3ec`  
		Last Modified: Tue, 08 Mar 2022 22:57:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2e9327114cf7c6bef30240edeb001e6427e4a56c4e02dddab6de0e9059e6d`  
		Last Modified: Tue, 08 Mar 2022 22:57:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d08fee42dd574617c8e2afc13341b9f2f0f41e514ba22b2e02ee4071b9e680e`  
		Last Modified: Tue, 08 Mar 2022 22:57:36 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7a0154e10f2b325fe2f7a72fe9d996391a31d99803cbfb2f9483312237cbfd`  
		Last Modified: Tue, 08 Mar 2022 22:57:41 GMT  
		Size: 83.3 KB (83332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe9764c2f7353b3ee9112c8f2a9c1fa7ca9ee81563237ee4dda986c99383c96`  
		Last Modified: Tue, 08 Mar 2022 22:57:36 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dee8f90d393ab6328d6193026e2854052808d03954034806ab6bc716f460031`  
		Last Modified: Tue, 08 Mar 2022 22:58:50 GMT  
		Size: 39.1 MB (39126378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a90b9bec258c3948b0970af86da418729e69e814059e6084e76c299f645de1`  
		Last Modified: Tue, 08 Mar 2022 22:58:03 GMT  
		Size: 60.6 KB (60560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.2686; amd64

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
