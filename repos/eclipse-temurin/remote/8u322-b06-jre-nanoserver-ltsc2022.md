## `eclipse-temurin:8u322-b06-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:6bb08c37349f5235f10b42085b63b910bc2ddd11adbc9313396cccbbe27679bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `eclipse-temurin:8u322-b06-jre-nanoserver-ltsc2022` - windows version 10.0.20348.587; amd64

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
