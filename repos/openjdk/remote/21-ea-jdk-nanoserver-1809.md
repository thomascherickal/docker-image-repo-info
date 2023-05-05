## `openjdk:21-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:9986734e6a60e791e6aff888c4c964230042bee3c7a93ebcb995612ac210b1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `openjdk:21-ea-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull openjdk@sha256:d18ba5d9ea4078e689fd066b6b1c1abb6726df63963940130c8e34e3a9d8032e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307216965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bad3ebc6fe9a2f565271da6d3451b7a9ed1491bcba6f600d07b9c586dc7a99f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Tue, 11 Apr 2023 23:45:42 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:45:43 GMT
USER ContainerAdministrator
# Tue, 11 Apr 2023 23:45:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Tue, 11 Apr 2023 23:45:57 GMT
USER ContainerUser
# Thu, 04 May 2023 23:18:03 GMT
ENV JAVA_VERSION=21-ea+21
# Thu, 04 May 2023 23:18:18 GMT
COPY dir:8073f6627b0b13d2d0e6669e88b700d52872f6d6985f68438081a66f0741b9e6 in C:\openjdk-21 
# Thu, 04 May 2023 23:18:34 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 04 May 2023 23:18:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959014ae4c354475658573dc2e10e98575d191deef98e1f23bf7cb9f4768408f`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b662327c70093bac13b7d07354fdbcd6967cbc13aaac870ca2e077fafefceb8`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9446ad09d009884e8a1db2085ef50cd6467dc3270eca7bac27fca70698013943`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 68.0 KB (68014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1335b1a9f9197626e9424d9d24737142c9d98659cc7f5510ca10378488d00b51`  
		Last Modified: Wed, 12 Apr 2023 00:52:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e7fe4ebf40e476c7815716b1232ea6a68c2db4bb2e309a1214493717147275`  
		Last Modified: Thu, 04 May 2023 23:20:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9d2496a41665261764e42a787c289e9e632225e5f4c2b2a1bf272f15a224f`  
		Last Modified: Thu, 04 May 2023 23:20:48 GMT  
		Size: 196.6 MB (196559925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee8f4eaa725529c66552f3c8a254e72aa2bd87ebc5ff23375e229f406817ea8`  
		Last Modified: Thu, 04 May 2023 23:20:31 GMT  
		Size: 3.8 MB (3793180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa7bc0feaa6f5a8e9f66c31a4a610cd92aaa04790ec14679c283ea9e43c4bc2`  
		Last Modified: Thu, 04 May 2023 23:20:30 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
