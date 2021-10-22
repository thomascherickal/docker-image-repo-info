## `openjdk:8u312-jre-nanoserver`

```console
$ docker pull openjdk@sha256:7c4fcf694e61fa422d6ef094145e61bc73ba8a7480c70e4b992e15ed32fbd563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:8u312-jre-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:2bf69d5e0cfda0cbb321081d68750546d6624f769d248d321d391be344643f5b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141049710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d690509ed32e99fd23ecf78ae9cccdacc835089d310f4b94500ea455360fcb`
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
# Thu, 21 Oct 2021 23:35:50 GMT
ENV JAVA_VERSION=8u312
# Thu, 21 Oct 2021 23:39:33 GMT
COPY dir:d01eca1f47b40119ea7401e87f8309ebbb3c59555f496ebfb4562b12d58cd948 in C:\openjdk-8 
# Thu, 21 Oct 2021 23:39:47 GMT
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
	-	`sha256:694c6ab16f054887327dcb17aab176758654c7f2ac6beeff6b4285100ce935f0`  
		Last Modified: Thu, 21 Oct 2021 23:55:16 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383ead589409f0f134eb7feb88a76141b51c09041eee872cd8ea85e8655f2994`  
		Last Modified: Thu, 21 Oct 2021 23:57:57 GMT  
		Size: 38.2 MB (38230035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00f15323c8288e1b7c8075506f291d91cdc0afc267a693eaf50443e2eed8f0a`  
		Last Modified: Thu, 21 Oct 2021 23:57:51 GMT  
		Size: 84.2 KB (84182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
