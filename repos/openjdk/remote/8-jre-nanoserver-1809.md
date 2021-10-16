## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:a8e520ad1c559e9c8362a24cc98362bfa199264cff5f2105dc14d2943cbfd200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:304619e76c4c5a60f907b52487eeba0bb57556ac085a855c699b5f25cad00617
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141038959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bfc5dabf61c9a5c4ac2d8b7ca11e38a03150a27ca3998844a7240c5447e698`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 01:09:13 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 14 Oct 2021 01:09:14 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 01:09:23 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 01:09:24 GMT
USER ContainerUser
# Thu, 14 Oct 2021 01:09:24 GMT
ENV JAVA_VERSION=8u302
# Thu, 14 Oct 2021 01:13:03 GMT
COPY dir:58006f68c4ea109e560c76de14918bddd55bac9724011203b6cdeb031fa20971 in C:\openjdk-8 
# Thu, 14 Oct 2021 01:13:18 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190b684414acbeec28d1f68830de15f4c3a4402880b57c5248346a7ab6a5ecf6`  
		Last Modified: Sat, 16 Oct 2021 00:50:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617e5deee7199f178e08bc5fe0bf5e1492b018a37dcd9d0de33612cb3c2fe193`  
		Last Modified: Sat, 16 Oct 2021 00:50:48 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fad13686c32e9b5b254194598fafcdcd366b13a8e9ab31fa04337bd964551e`  
		Last Modified: Sat, 16 Oct 2021 00:50:46 GMT  
		Size: 68.5 KB (68460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b862b55c85cb12a4113f1fc798a6ac40c83f67a1b64d83aa2be4dd2ce22c93`  
		Last Modified: Sat, 16 Oct 2021 00:50:46 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccee7cd9c5d40a26767d50095834acce1babee1f96c431c0584994e3ad4d91f`  
		Last Modified: Sat, 16 Oct 2021 00:50:46 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e96c0e8b99258dd64dbf22dc2725f9d8c28c167f099edda78a887f285ee69d`  
		Last Modified: Sat, 16 Oct 2021 00:53:28 GMT  
		Size: 38.2 MB (38223191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02c001462ea9d47df946894815a12b5072bdc5098a3a6c623aa100333b3438b`  
		Last Modified: Sat, 16 Oct 2021 00:53:21 GMT  
		Size: 80.3 KB (80291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
