## `eclipse-temurin:18-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:3f72ea34d2628a8e5b70b8861a996d026123d384a8593924cbe226f9b4c77466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-jre-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:ba53cdb2cf41c7272cefa2935d58a10561d058aaddf84dfbd9415d3744668d28
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.8 MB (160767356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28241b87f87cdbe1dc28a8f1889aed22aee726aecf6ced591532b4d81d9c6f2a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 04 May 2022 18:28:26 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:28:27 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 04 May 2022 18:28:28 GMT
USER ContainerAdministrator
# Wed, 04 May 2022 18:28:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 04 May 2022 18:28:35 GMT
USER ContainerUser
# Wed, 04 May 2022 18:29:18 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 04 May 2022 18:29:27 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:924a7c42e559a85c0bc74dbb028ddeee43fe67b0f59c81c60cbda0082e0e3ae5`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089a88f54de05890eaab4cbd37399afff42f7c5a9f550a19ed7962758a221939`  
		Last Modified: Wed, 04 May 2022 18:36:11 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d16e4f5a8aeb16031deb5c6584de9e4305697e9e1a3d44c591d95879e7d09a`  
		Last Modified: Wed, 04 May 2022 18:36:11 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f7366067083ae01419dd31e6e105cf84b82a5b7f91b812bc60cfb58c92a4c`  
		Last Modified: Wed, 04 May 2022 18:36:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b858cdf486d22d72c1a9c9ddd294e947fd16a4004d6428626dec088a50440f2`  
		Last Modified: Wed, 04 May 2022 18:36:09 GMT  
		Size: 82.2 KB (82245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee2117aee9f2bae1b8685e7023b8ada6f81a5ef6e467c3fe506e7fa016a97b7`  
		Last Modified: Wed, 04 May 2022 18:36:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5760b1a774361203c9a2389ced9a485c5ef4bcec4819c4e66ce09ced6c2196e6`  
		Last Modified: Wed, 04 May 2022 18:36:49 GMT  
		Size: 43.0 MB (43038209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193987a206110b8d10ee4e61d7383173d629b9f6b676b3c80b211cb0c49f2f6c`  
		Last Modified: Wed, 04 May 2022 18:36:40 GMT  
		Size: 61.9 KB (61865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
