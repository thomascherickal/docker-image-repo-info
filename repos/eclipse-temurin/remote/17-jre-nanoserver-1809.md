## `eclipse-temurin:17-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:4b66505d7dc52049a2f4a9c2d979720df2269feedfd78de871e826aa0783d3c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:17-jre-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:3e3ce9af6f080765d437bd3e84ca22915baaa35cc502c1755cd8deeff0ad181e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.9 MB (150910784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5040b199ac266d5216bfd7b8d116ad2c72e8fd3e671e00f7e4188e3f482265`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:28:40 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:28:40 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 30 Oct 2023 23:28:41 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:28:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:28:48 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:32:45 GMT
COPY dir:d3f692ac99669197443250e31cbc5c2f5282787fd78589cc9b6c2e91236738f4 in C:\openjdk-17 
# Mon, 30 Oct 2023 23:32:55 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544ee40eb274d2cf11d28d99d0c8494a24e00f0f1137b7e564be49e87156f107`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161906f3b49bd6fd6c057a7ab136803617df69e360227bf85071954cbaff5bd`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9577e25e1dd402829dc73e75680c93ecc3ab8b98e0ab4a0426d280e445f0b3dd`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8466f9d333da539e80924cc14314d112e43eba15e91d933a916db00a4544c4ba`  
		Last Modified: Mon, 30 Oct 2023 23:51:27 GMT  
		Size: 68.3 KB (68304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8ac5c462e2a023aec1e4bc0979a6aca435b4e18a061c38f710d3ba7720f7a`  
		Last Modified: Mon, 30 Oct 2023 23:51:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda561ab329c5755dbe54a96f2ce9e09784d62611245f88fa050631a66943303`  
		Last Modified: Mon, 30 Oct 2023 23:52:42 GMT  
		Size: 43.4 MB (43397395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4212ba31c15c74e58d05bb7337a1dfd0eb9553aabda257ba62843d7a88c678e3`  
		Last Modified: Mon, 30 Oct 2023 23:52:35 GMT  
		Size: 3.0 MB (2974789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
