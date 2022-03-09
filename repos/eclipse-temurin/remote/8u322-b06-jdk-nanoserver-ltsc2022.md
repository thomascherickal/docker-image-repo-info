## `eclipse-temurin:8u322-b06-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:cd72a45cbed41f3b759ffb720404a4e7abd92364e234f0c836f70fc70c441408
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `eclipse-temurin:8u322-b06-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:8dcc535ba1f01ca684193db76a86f6281e6f6653e03dcfae5bc73321257ff4ba
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217835440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a7c8c82561d6ac7dc98164417b2845698baf86f6971a9af99c7843dfc43388`
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
# Tue, 08 Mar 2022 22:26:33 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Tue, 08 Mar 2022 22:26:56 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:191f7537d99c70778e40c3c1e660ce8b0d6d1b440ff29223da4b3b55ef00c3ff`  
		Last Modified: Tue, 08 Mar 2022 22:57:49 GMT  
		Size: 100.2 MB (100200156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7b6b4a5db48652bfd929033eb78c5e01fc21d17243780f59aa337b212e481a`  
		Last Modified: Tue, 08 Mar 2022 22:57:36 GMT  
		Size: 60.7 KB (60706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
