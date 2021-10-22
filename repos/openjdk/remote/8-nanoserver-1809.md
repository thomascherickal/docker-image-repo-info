## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c41c88807ae767a964c2c953a0dab6f295164138a2f9e6c7fa4d7bf782fc7c1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:cd1cb476aa8934c0819f1783758df084f6d910bddad3a0e13f9a1731c30292fc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203887531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c844bd2a023dd018b46dfb625c157ad659340b2d3925c85a32160826594246`
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
# Thu, 21 Oct 2021 23:36:05 GMT
COPY dir:3a5581b2700e30ac96b7aaa667bdc25cdca1d6451f9f3d58913682ddf8d74e71 in C:\openjdk-8 
# Thu, 21 Oct 2021 23:36:23 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:e9fdc79270d23858a410f2b412d86b9acc880143b1291d13937b3cc9a7903d9a`  
		Last Modified: Thu, 21 Oct 2021 23:57:06 GMT  
		Size: 101.1 MB (101070650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010d0c5d162640ebccf10c5a486fc80fbe1bf42aba90c41e8b58b8e45c6fb1a0`  
		Last Modified: Thu, 21 Oct 2021 23:55:16 GMT  
		Size: 81.4 KB (81388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
