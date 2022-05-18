## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:5e25b065d2638bb6f463b41db4a64ccf43c273dd2e26893c1a6be431c5c96b29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:0d11e590713961381f7092387ec98aa81369f69117c3077f7c633b0d13c43de9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.1 MB (292062079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8cffdd19a44e44a244a9cf29d9393c5b988819a451d6b5f6739b26e286cfe3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:07:30 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 11 May 2022 15:07:31 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 May 2022 15:07:32 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:07:41 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:07:42 GMT
USER ContainerUser
# Wed, 11 May 2022 15:07:58 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 11 May 2022 15:08:24 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:08:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8743647b8ae81c92754d445c24fcc8939c32453feaafa85fefb9b276cab329cc`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bab84fbf268fee41493c0a1d9cf46b40b6d040166aba8958fbc2c361b4f466`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c28f4021ca921cb65e2fe828836e1a891b3269a35543193d4c8f1932c94cf5`  
		Last Modified: Wed, 18 May 2022 13:21:42 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4675ebe79379c89ba27a3579f9aef7ce52b76bad0e4978160afc55ee6573a6d7`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 70.2 KB (70154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1be201dab22ad99a45344d8dd0c83a049ac7f66c67ee69d254e23f83444cd1`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526981b83c5987ee605ff2fee424bd116f427296e9d92fbd219b918f3abbd22`  
		Last Modified: Wed, 18 May 2022 13:25:02 GMT  
		Size: 185.2 MB (185189434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fb8535124aead58723fae0c475eca7324aae8697da99a49c92a4561cdd122`  
		Last Modified: Wed, 18 May 2022 13:21:44 GMT  
		Size: 3.7 MB (3661732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fa3f936e0678af6ce3e38ed6e89f311708e27277749c0fe7e2ac014295785`  
		Last Modified: Wed, 18 May 2022 13:21:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
