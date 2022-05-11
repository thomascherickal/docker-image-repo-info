## `openjdk:19-ea-21-nanoserver`

```console
$ docker pull openjdk@sha256:b8c16e151754cd73c7a333342d9d21f7ce1284febe96526f945d18f6bec4c33b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:19-ea-21-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:277d877552028ec523a892dc211deff1b0e890cacc2fc72d613238f63556a9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296597463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a389d3062f6ded1f7465acfe792ffd7a9277de74b21b6d2f0a913d3c63a4452`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:33:35 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:33:36 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:33:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:33:48 GMT
USER ContainerUser
# Wed, 11 May 2022 15:33:48 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 15:34:03 GMT
COPY dir:36e2807462a4fa7d77ed8add626cd5e858674e5a65a735b72b6a826136082fce in C:\openjdk-19 
# Wed, 11 May 2022 15:34:21 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 11 May 2022 15:34:22 GMT
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
	-	`sha256:27258317e27e0cfabcf779836e0e38e0809f5ba5b2e2ce61b0c4761494eabf2f`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f575ce9dbc595a6266a2d907de169473af97a71414d6a81d122bfc9cd5e39`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40175500d750084c8212d8ea8f70d757ec3255fcb2fe588e2663c8a405187094`  
		Last Modified: Wed, 11 May 2022 16:00:33 GMT  
		Size: 74.5 KB (74495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d665e0106401630d154ad3a944dc128966740b1e1b21d2fbeab345b8da177a`  
		Last Modified: Wed, 11 May 2022 16:00:31 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690c36864583efccf0a16a2f77df262818abb856561173b1f8a9384dc20254ea`  
		Last Modified: Wed, 11 May 2022 16:00:31 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ead10d0dca6d706d3404e628bf8f26be332138545ae956128417e9c4625cf8`  
		Last Modified: Wed, 11 May 2022 16:03:52 GMT  
		Size: 189.8 MB (189826383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da1e298db552ae9fea0bb3361a894255a55ef9b00ad72c484aaa2360dce8acf`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 3.6 MB (3555835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5396013fa0f5c53dc3431ddb1e3ef40190020e9ceeccfadd593d5f5fe49e090a`  
		Last Modified: Wed, 11 May 2022 16:00:31 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
