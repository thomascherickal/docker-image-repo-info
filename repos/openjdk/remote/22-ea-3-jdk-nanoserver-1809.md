## `openjdk:22-ea-3-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:50a24efc1517b8df7a94a0f3eaaf38ecfcc755b01ee29d4330484cf3126da1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:22-ea-3-jdk-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:a62069d968bffc5a23d20ec8130595e176fbce3b7bb404e9ff06317f3ab9846b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (307014588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8e5d3951353760bf444e1364b739dee63cf1b0172cdc54c5dcc739da22a304c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 20:28:06 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 14 Jun 2023 20:28:06 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 20:28:15 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jun 2023 20:28:16 GMT
USER ContainerUser
# Fri, 23 Jun 2023 00:36:54 GMT
ENV JAVA_VERSION=22-ea+3
# Fri, 23 Jun 2023 00:37:09 GMT
COPY dir:8a420f20927ee12c5664336246fe9e7981c10034572e95cbd352de42199c9295 in C:\openjdk-22 
# Fri, 23 Jun 2023 00:37:21 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 23 Jun 2023 00:37:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816e92368fa87f9798749d97162f386f464e5cb0e4a668b35ac6929b5f9bdbab`  
		Last Modified: Wed, 14 Jun 2023 20:35:15 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d241a7335cf0716c38d3ab576802c34648d69d25e847638aa7db2132e881461e`  
		Last Modified: Wed, 14 Jun 2023 20:35:16 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6d759053b47bb836ae8319abce7846d93cfdf210fb3e4b0bcce271fbda6d9e`  
		Last Modified: Wed, 14 Jun 2023 20:35:15 GMT  
		Size: 74.6 KB (74612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3005cad1749dc64b4a46eb5a441e05083078d3075dbdb1cac2beba0044199668`  
		Last Modified: Wed, 14 Jun 2023 20:35:13 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6841f3b0c3b74df23b795a8d20d560e07f487c4bf799f245113a8d822e8c0531`  
		Last Modified: Fri, 23 Jun 2023 00:42:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200522c9bebeba1c962051a4ad7900c74cb74bdfe18bc219f617ab52b97e06a`  
		Last Modified: Fri, 23 Jun 2023 00:43:04 GMT  
		Size: 198.8 MB (198766072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75cb68ee9fd04e2f9879b73da3322acdbcb08044000a841f69df4d256cb3465`  
		Last Modified: Fri, 23 Jun 2023 00:42:45 GMT  
		Size: 3.8 MB (3769258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27670d3657c3f4df34f069106611a2269120aca09b554d10efce1efdb7e5c4bd`  
		Last Modified: Fri, 23 Jun 2023 00:42:44 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
