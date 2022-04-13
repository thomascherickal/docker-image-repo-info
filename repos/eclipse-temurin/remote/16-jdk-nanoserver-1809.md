## `eclipse-temurin:16-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:1f9f2b72b10f09fdd9a29495f75d8c94e27a34e612cce401aeae68accf0c75f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:16-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:50a4d4d266cdf206257da493f03f73cd4e3ac9d7ed061b4b78a727947242b01f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305595548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701afb6ca3a313568bf69112cdeaf473e2e2a64373e899613fc3b526567826b7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:32:08 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 13 Apr 2022 15:32:09 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 13 Apr 2022 15:32:09 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:32:16 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:32:17 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:32:31 GMT
COPY dir:9a7ef5975d9ba9576c4744dc049616bbcb218f14c3c0bd967851cd46479d6134 in C:\openjdk-16 
# Wed, 13 Apr 2022 15:32:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:32:43 GMT
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
	-	`sha256:209812e7f5982f4b180146b034a1c767b5f3bcc14b9412f365e4655204cf9ca4`  
		Last Modified: Wed, 13 Apr 2022 16:22:13 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3137a5abef69755caf360633bcd164ffb6c08fc09234a95c72bb445850874e7e`  
		Last Modified: Wed, 13 Apr 2022 16:22:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8e70fa09d0c04b115a3e29258e3367777189f47e996b0718f80fb75344642f`  
		Last Modified: Wed, 13 Apr 2022 16:22:12 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f70172d26662be7d028b7d7c4b9942b86dc99eacaece9696f5f986b1f4fa61b`  
		Last Modified: Wed, 13 Apr 2022 16:22:10 GMT  
		Size: 71.1 KB (71137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac0449fdb0e7e9bcc554bb4cacdaf6dcdaf0610c8710bb7f51ae6892e8d555`  
		Last Modified: Wed, 13 Apr 2022 16:22:10 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954b70a8c9b3d42ee16082a995ad69f9ccc8031a19dc3455bfe1a2ef3cce310`  
		Last Modified: Wed, 13 Apr 2022 16:25:43 GMT  
		Size: 198.8 MB (198756192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ef75bbf40f0b6c037ab29572a28fb13872e31357992477e3367522a1bf616b`  
		Last Modified: Wed, 13 Apr 2022 16:22:11 GMT  
		Size: 3.7 MB (3665223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6bb7fc8c8c278fc3a636fb22c30912beb69f6d34385162560e7fd3de4fe5b`  
		Last Modified: Wed, 13 Apr 2022 16:22:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
