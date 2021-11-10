## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:2c2ff51a6f849a8b269af941488706fcd360fb3f2516be5e8b4567250120c8d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:a0fc26b7c4e001dc87f56134e891782ad6569ff5350d1b775d26d74753bd64e1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156372318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e12878914b71d8e05daf18415e032ee51bfe97b7ee96b9cec0a7ab6206ac379`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:52:20 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:52:21 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Nov 2021 17:52:22 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:52:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:52:36 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:53:15 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:53:28 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ceb9b6cf720f75473e3c41307d287700ff9e2fcbb1e7fd036ed7a78a6c64e4`  
		Last Modified: Wed, 10 Nov 2021 18:53:57 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61655ff5d6ffb4e9b28c5bb62ef4e6838797460f0b1136f043b2cd0599eb5190`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f8ab0cd19e99cc99b76ace65f501d956fbb5509b9973f1a12056915e44440`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52fd3b2829a4a90396e730bb05b5685ca3e796a913593b91dda4cc283e5e8b6`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 99.2 KB (99243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1743a12c5b583262adb490179aeb5cb182f8fe9389663880f95527c27db067`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb61e0c01de5c281535eb310414e9aef8bbb926d6f7beadb9c476047209bd3b`  
		Last Modified: Wed, 10 Nov 2021 18:54:25 GMT  
		Size: 39.1 MB (39081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a65665d9dbd44743f8aaeeeeb8e7600716fce59cf6257b2c5a1c156dd8200`  
		Last Modified: Wed, 10 Nov 2021 18:54:19 GMT  
		Size: 68.6 KB (68577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
