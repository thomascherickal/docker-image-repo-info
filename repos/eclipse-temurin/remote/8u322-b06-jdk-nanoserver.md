## `eclipse-temurin:8u322-b06-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:0ce2d3101ac7be1eeab2e7ca6600a1189dfd7c05300b522283d0c641d6c6c627
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:8u322-b06-jdk-nanoserver` - windows version 10.0.20348.587; amd64

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

### `eclipse-temurin:8u322-b06-jdk-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:8329478593a051336e0980b22d5ce01eda47abfd6f01ddd4f5651be5ff6cfd97
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203437072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0410b1ce72037cd0bdbfd2cda78c8ce34710ce303efe2f11be7e6bad12cf9b9e`
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
# Tue, 08 Mar 2022 21:56:47 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Tue, 08 Mar 2022 21:57:04 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:773be34cda0449a4e20d5f908fe200cbcc586310dddc221a280097bccfde2dce`  
		Last Modified: Tue, 08 Mar 2022 22:37:31 GMT  
		Size: 100.2 MB (100216460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bb8cd0491943d8b11ee97b73d44d3c675fe5f6d8a2a6e01ff8891817f68c7f`  
		Last Modified: Tue, 08 Mar 2022 22:37:18 GMT  
		Size: 90.7 KB (90709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
