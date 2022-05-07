## `openjdk:19-ea-21-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:1d37ce86a30a9d94ec36d035528eab9f2ff1632c8eeee1f0802a22e379f9eb8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:19-ea-21-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:8a5fff6b0ba8342591a260f13fcbc425e88d1b7643ffe9d0118940f621c64924
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296556825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642163e2ba4bcf73b9f2ac56616951cd4a8fc322ae173e10e81f1ce0e6db978d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:00:37 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Apr 2022 17:00:38 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:00:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:00:44 GMT
USER ContainerUser
# Sat, 07 May 2022 01:18:44 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 01:18:58 GMT
COPY dir:36e2807462a4fa7d77ed8add626cd5e858674e5a65a735b72b6a826136082fce in C:\openjdk-19 
# Sat, 07 May 2022 01:19:11 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 07 May 2022 01:19:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4644baf69a04abfb80da969c1fb009552c461553f3672bd4e787c0ac7c37ea`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61095df7d33e436b0d9cb0052f433e155a897f4278b9dc0a8d13582d6cad38ad`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2110ca10faf88314f61157ce6bfeb157b8b8eebd74be6f0a78f2f7b82c514a`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 68.8 KB (68813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd03d4716f16fd9ebec77b5cf5099ed25d889884b5a06da589ce896a7db47a15`  
		Last Modified: Tue, 19 Apr 2022 00:53:49 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14062e874d0106d48137fa3f519ac74d6f8c9c70eb5f6b47a1b25b63849a3232`  
		Last Modified: Sat, 07 May 2022 01:30:43 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320eb99112e5037e983bcfc3afcfac37cfa1330034fa6325b3f2b82aeb202a2a`  
		Last Modified: Sat, 07 May 2022 01:31:02 GMT  
		Size: 189.8 MB (189818856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbb57890260366a5df211dcc8a630389b40f34d549d8dfefb700add21e9dbae`  
		Last Modified: Sat, 07 May 2022 01:30:44 GMT  
		Size: 3.6 MB (3566221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd9d3e7e8ab029911a7dc3cee37bbe5b5b85bda84b48f46cd96197b1aed4e94`  
		Last Modified: Sat, 07 May 2022 01:30:43 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
