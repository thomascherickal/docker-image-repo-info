## `openjdk:8u302-nanoserver-1809`

```console
$ docker pull openjdk@sha256:725830be44a0d78f26f0dbdf70c39f3101f2f4d5c2115db0afddeeab10c3d330
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:8u302-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:6f6f3ae33a66676011c06ccd1dc3039ec98d91ee4a0e80cee74b5fb43e07589f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203888243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39584324c0e378f1cb8ac5ae389ca9228161afe421307f2d816ace7c4d1a712`
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
# Thu, 14 Oct 2021 01:09:41 GMT
COPY dir:82904e6295068720536f940f57626186b2820e368b810e639bd5a3957d468086 in C:\openjdk-8 
# Thu, 14 Oct 2021 01:09:58 GMT
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
	-	`sha256:bccee7cd9c5d40a26767d50095834acce1babee1f96c431c0584994e3ad4d91f`  
		Last Modified: Sat, 16 Oct 2021 00:50:46 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee9e3210a5aa2861cc4fcb7275759985dc16deff20cac20f443cd8619c62cf1`  
		Last Modified: Sat, 16 Oct 2021 00:52:30 GMT  
		Size: 101.1 MB (101056040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f050a67a5cd082f5667e37cda621f451cdd0a23c8a33d259a6aff1416abe326a`  
		Last Modified: Sat, 16 Oct 2021 00:50:47 GMT  
		Size: 96.7 KB (96726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
