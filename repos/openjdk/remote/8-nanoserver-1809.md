## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:aab2eed97731be0324282e881a41c88486e1b2c24b2990a0abc2d0a61d0d205b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:d2ef8f05ae960ff29b6b27a59f1498db4e2c00a53e913e0f98843441dc317e31
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.3 MB (201254354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819c317b9be2d466f6841d2fbaaf828d33438894a402321d292cf41df014837f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:28:05 GMT
SHELL [cmd /s /c]
# Wed, 12 Aug 2020 16:01:37 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Aug 2020 16:01:38 GMT
USER ContainerAdministrator
# Wed, 12 Aug 2020 16:01:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 12 Aug 2020 16:01:49 GMT
USER ContainerUser
# Wed, 12 Aug 2020 16:01:49 GMT
ENV JAVA_VERSION=8u265
# Wed, 12 Aug 2020 16:02:14 GMT
COPY dir:3c2880b061bc00940ee162754a64e55567e0dbb10e65b749277b54fa005ce8de in C:\openjdk-8 
# Wed, 12 Aug 2020 16:02:33 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1c7c341c7a3d0c7b6e849b6faec560815682d07ce87df2e4d1e83f928aab306b`  
		Last Modified: Wed, 12 Aug 2020 16:10:21 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4daf365d1451ee22d41b366a1ff5ae969d68435a4891cc5058e83d868b008eb`  
		Last Modified: Wed, 12 Aug 2020 16:23:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca485eb3d3fbc53b7bfe83c1550f9bec33fdc0153a7e297dbe84fc77f5c310a`  
		Last Modified: Wed, 12 Aug 2020 16:23:30 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7252510ed8c3f762146994311ff0bed65ea719de5018c2f7c41e62543c26f`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 66.5 KB (66516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3df101f8092504a16a2b624e67e78b3fa8131c3908c1c309d5f6d70537afedd`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 935.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae04b3252587787aa96faab00ea2ab17d328bf541c96c8e11997c5095fd6aaa6`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd143ee2775bddd591fb8878e3ddd2af2aa4a16b54ecefd216b0c94656d6340`  
		Last Modified: Wed, 12 Aug 2020 16:23:46 GMT  
		Size: 100.1 MB (100111051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0040982192eac204fd05e0f7eab16d0c937cb127ca996e0266f4cf1bfd33bd`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 87.4 KB (87400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
