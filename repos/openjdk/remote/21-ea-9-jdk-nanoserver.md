## `openjdk:21-ea-9-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:e30c32bbda46c98434171853da228475e2fef69a49e5c0c9c03bed7203c831ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `openjdk:21-ea-9-jdk-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull openjdk@sha256:78d4e2554151dfb6656cc4bef3445ccc320e97f0278ffe73066d23ced30d0c98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.7 MB (304701522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59b863a0aa80fcf45b41ea0788b547105bf18b5d680006aef3e8f1fc4a3104ba`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Thu, 16 Feb 2023 02:20:16 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Feb 2023 02:20:17 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 02:20:26 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 16 Feb 2023 02:20:27 GMT
USER ContainerUser
# Thu, 16 Feb 2023 02:20:28 GMT
ENV JAVA_VERSION=21-ea+9
# Thu, 16 Feb 2023 02:20:43 GMT
COPY dir:d22ed295da240dffc46c261d95a62ee269aa2940a1a41af4173a504de0e076b2 in C:\openjdk-21 
# Thu, 16 Feb 2023 02:21:00 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 16 Feb 2023 02:21:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b040b2f53926e6a02088ae0173e36f1f01b75c581f435607dd2f86dfe095f4a`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0134c2e5e080e208ed0917cd948446b60048729433bf731850e4165e426977c`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf352af9ffad203bc10ae043af50fee20ca5c0e02a370dcc2b040c702c9d48f`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 67.9 KB (67900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58adc24996cad294b1ceeed12449ee5750c4442dfcc5e3135984239942ba8503`  
		Last Modified: Thu, 16 Feb 2023 02:29:13 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6e33366df12d57318c17a89abaad6bf49636a34ab718a99d3ba5d2e89ff462`  
		Last Modified: Thu, 16 Feb 2023 02:29:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ab33f98e5cfa722e62e02748a9c03262f6b59709fcf56f041f525e02face8b`  
		Last Modified: Thu, 16 Feb 2023 02:29:35 GMT  
		Size: 194.2 MB (194156822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f86b50388196f4e56da5452aaad76beb0621babd39d02220a4157cb594b7fe`  
		Last Modified: Thu, 16 Feb 2023 02:29:14 GMT  
		Size: 3.8 MB (3795038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb21b61e25b4902e097bd03932ac0c0495f5c7cdbe65175c770d076ad3163b94`  
		Last Modified: Thu, 16 Feb 2023 02:29:14 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
