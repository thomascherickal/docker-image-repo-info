## `eclipse-temurin:18-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:bb33366cddc98a22984233ab556790a7bdb511924a83c15e2775333145e4e0d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:18-jre-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:a66a04025f95754a869d33bd0df64ad4c0c62a9be74f5d7e25c27271b4ce91ec
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.1 MB (149140694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d61a65533523e1c78072fb084fd3d3de5656acbc199203c20159b88ba67b9e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 04 May 2022 18:23:03 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:23:04 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 04 May 2022 18:23:05 GMT
USER ContainerAdministrator
# Wed, 04 May 2022 18:23:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 04 May 2022 18:23:12 GMT
USER ContainerUser
# Wed, 04 May 2022 18:27:38 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 04 May 2022 18:27:48 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1818cdab77f23e78fedaca52a20efe1c4ba35571fb089c70e1485124b9c6145`  
		Last Modified: Wed, 04 May 2022 18:33:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77646ae8dc09eb94667a43ea3487777f6cc340f4aaf6c909df70299066d9d371`  
		Last Modified: Wed, 04 May 2022 18:33:29 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7102f2da8b5b2796607c79458ec46fa80513872248c745ca845aca54bd2163`  
		Last Modified: Wed, 04 May 2022 18:33:30 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66b464e0ea5b83f563c471243fc90144f3895080f5cdb204456348cdc10af`  
		Last Modified: Wed, 04 May 2022 18:33:27 GMT  
		Size: 72.4 KB (72386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362058c540505251e6ea236372b1a3e9b786fe60acaa0b59a4079cb357fb05bb`  
		Last Modified: Wed, 04 May 2022 18:33:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab88679171d6bd2294e2b1218bcdb2fb57df068ab22f06e68481baacfa0f478`  
		Last Modified: Wed, 04 May 2022 18:35:54 GMT  
		Size: 43.0 MB (43048651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa1b966bb3aa2be70011731ab1d7e230e33f11b4489fcb6571038cb614bab43`  
		Last Modified: Wed, 04 May 2022 18:35:46 GMT  
		Size: 2.9 MB (2917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
