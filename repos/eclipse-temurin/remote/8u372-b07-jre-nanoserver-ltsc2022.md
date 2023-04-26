## `eclipse-temurin:8u372-b07-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:ee1efd9b51b7e959a910ec9f764a49b6aa67c10aa7605c35313923d7285806b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `eclipse-temurin:8u372-b07-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull eclipse-temurin@sha256:943764c79cd4704d45341c588cd353c9700431583518e0ebb675bd722b70b773
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb4f92ebe818c1206d693026b0f0021615f5e261a0195717d30adb03bfdc4fd`
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
# Wed, 26 Apr 2023 19:53:14 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Wed, 26 Apr 2023 19:53:25 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:705f9ecde956ffa7021589a63652dcfa3754dd4de91c96180cb8f8b8295f7d83`  
		Last Modified: Wed, 26 Apr 2023 20:10:05 GMT  
		Size: 40.0 MB (39956206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c1c236a5a17be8bd5a2493bf6cfce45513692f41061fdf1c3f1e1f5cc41e68`  
		Last Modified: Wed, 26 Apr 2023 20:09:58 GMT  
		Size: 70.4 KB (70431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
