## `eclipse-temurin:20-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:bfed69bb12aaa9e6a18bb1b55b14b0bfab0bd8e46450a4de056dcb4cea8e9a33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `eclipse-temurin:20-nanoserver-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull eclipse-temurin@sha256:94b622810267b39590c9fe65f10f59acda316b55b74b23f06dcf6c7cdf2e961d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.7 MB (315664976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e38eced08677b9c2c67bd95464dad2fe0991d3893aeb2d7fb9ded5fc8bb58062`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 22:10:51 GMT
SHELL [cmd /s /c]
# Mon, 24 Jul 2023 22:34:58 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Mon, 24 Jul 2023 22:34:58 GMT
ENV JAVA_HOME=C:\openjdk-20
# Mon, 24 Jul 2023 22:34:59 GMT
USER ContainerAdministrator
# Mon, 24 Jul 2023 22:35:16 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 24 Jul 2023 22:35:17 GMT
USER ContainerUser
# Mon, 24 Jul 2023 22:35:34 GMT
COPY dir:4ed074865171ba014f3c2f68f57ad2bb21a4dd6e4cf7ff9654ee6c4c6e5176c0 in C:\openjdk-20 
# Mon, 24 Jul 2023 22:35:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 24 Jul 2023 22:35:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cc0a26bd90fcc4d863317c36d7ffec77a0a82a905697204d4dcbc76ec13b3920`  
		Last Modified: Tue, 11 Jul 2023 20:10:45 GMT  
		Size: 120.1 MB (120056465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11750b624a775aa3c21a13406dfc54458855b8684e21efba5bbb9b27ee0b12`  
		Last Modified: Thu, 13 Jul 2023 22:28:35 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df03e5a85a6761fb9efe6df02bff339628d33192479fac4f4c80765ecb467eef`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb4d53565cdd7fcb858eea61889381d14090947f03297df736e4c9cb1eb0b0a`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b41305755dfc1b9134e1943811949039f0f83b9c472199fb2a1f87bb4fa648`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfdf758fe560a8a115eed1641a54aa1d98588b326ed28c0f4f9ba9f13d2d528`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 78.7 KB (78687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610d1be704af1f3692c5ba787db39540820b0f50a7540e0e953478d58bf4414c`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7cb00aae4a4c28a75ca89c5b8713bdb43681cc2220a6e565171a6bc52b99c`  
		Last Modified: Mon, 24 Jul 2023 22:42:18 GMT  
		Size: 195.5 MB (195461699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3fd34fb50c0cf264fdfe7ceb010bc5a49c21cd5ed28d6cf4ae0f312828baed`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 61.2 KB (61157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34676e824c6cc0040c9389963caccd5f94d71e10800ebbacda6ca29e872796c`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
