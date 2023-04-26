## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:e7bbb0dfd1de6f262ed4a840569728f09f5c05b503c5d74342fef8aa29b24c90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull eclipse-temurin@sha256:8c9de26c8f2785833f646948293431289b2e9c07b7defdeb481fd0a341ca8ee1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223940286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c5a1851eca98469d87d5a84bde2ab3b31756b9bb597af1411f93a3f41e686b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 01:42:21 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:52:17 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 26 Apr 2023 19:52:17 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 26 Apr 2023 19:52:18 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:52:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:52:33 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:52:43 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 26 Apr 2023 19:52:56 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8058ec80ac2516d001291dea383d4abfa22416397a4c869e6fd79c0d4b64565f`  
		Last Modified: Wed, 12 Apr 2023 09:45:40 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac65bac07b0012556025ffb9bc1a66ef7ae07458f7b70e106efce9630f14bd62`  
		Last Modified: Wed, 26 Apr 2023 20:09:38 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d190fe6f81cc703bba42f10badc6e6338500a7ac2ba18a714017782b882bce3`  
		Last Modified: Wed, 26 Apr 2023 20:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d33e7aa70b8aef5760880fd5a8203e45f1fb672a4afed3a5dab7ceeeebfee7f`  
		Last Modified: Wed, 26 Apr 2023 20:09:36 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d58687c94e13392ca62f866e11a6fd92d78eaed2bdd7c04ce21ebd70fa69dc8`  
		Last Modified: Wed, 26 Apr 2023 20:09:36 GMT  
		Size: 94.8 KB (94835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a892db31b6e67caa42bd76ff3ada42891328d9b24868af83e83236c914a9f39`  
		Last Modified: Wed, 26 Apr 2023 20:09:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b795db7785853349e8438b7abbce2dc123387162347041700e99dd71ad4a91`  
		Last Modified: Wed, 26 Apr 2023 20:09:47 GMT  
		Size: 101.4 MB (101440342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3c3b0e263bc674d36b781765eac59327f0af44c554a1e021470deb5c356800`  
		Last Modified: Wed, 26 Apr 2023 20:09:36 GMT  
		Size: 70.5 KB (70506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
