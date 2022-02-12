## `openjdk:18-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:261bfe894daa8981137e3ff2fa6b0ba24a79ec38f477ade7a045578f6f0d6ce4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:18-ea-jdk-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:c85ea936da3b25b8c57c806542439d31c65891210ae51b007a406e82c2110195
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.7 MB (290674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ea24bdd161ef0385c6bace1825d07a3724438eec11985ece39aa45fef915ed`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 18:51:12 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 09 Feb 2022 18:51:13 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 18:51:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 18:51:21 GMT
USER ContainerUser
# Fri, 11 Feb 2022 23:23:24 GMT
ENV JAVA_VERSION=18-ea+35
# Fri, 11 Feb 2022 23:23:55 GMT
COPY dir:e730a8fc726f71f1543d4e586fbdfe295256bbd7bf7409bef8fada32981c7046 in C:\openjdk-18 
# Fri, 11 Feb 2022 23:24:19 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 11 Feb 2022 23:24:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5a7f567e84a5a148036156650a47ef7eec0187f17e880d3b475e51dacd70077b`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadac251c3aa431173a9a814bbf22a1c4c7cc50c68fe4a5f5b4592a6f7eb2ab5`  
		Last Modified: Wed, 09 Feb 2022 19:22:54 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9859cca3203f733180120b02358ffe6dcf5529a6f520497fc7c9b10faee52`  
		Last Modified: Wed, 09 Feb 2022 19:22:54 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a2fdc8fc9937a202c512de06d672695c8ab28ea5e9dc2713829471e0624e6a`  
		Last Modified: Wed, 09 Feb 2022 19:22:54 GMT  
		Size: 75.1 KB (75096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984c82eb4195ae947a96ff3d0c602b4ade866b01484e6e1b42f60f69163cecbc`  
		Last Modified: Wed, 09 Feb 2022 19:22:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d64b9bf70bde80c6ed1d7a4a6b60775a9b18c5d019fca8efec987e47e5fb5`  
		Last Modified: Fri, 11 Feb 2022 23:42:49 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b73670080f730a10fdccfbc49f62a5373733f7b4f81a708e2997c2f3c21c68`  
		Last Modified: Fri, 11 Feb 2022 23:43:08 GMT  
		Size: 184.0 MB (183971436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11448d79285b149b90948bd4918038be73edbe02659b6d55633cffab48689baa`  
		Last Modified: Fri, 11 Feb 2022 23:42:50 GMT  
		Size: 3.5 MB (3534112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc6909f7ab63a9994c82f029d6e3daaed541798e6f3a334bcc1ea6dea8ed4f`  
		Last Modified: Fri, 11 Feb 2022 23:42:49 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
