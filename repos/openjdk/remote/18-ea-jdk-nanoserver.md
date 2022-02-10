## `openjdk:18-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:ce1405b3bbe5ff5af02ccef59f655612e3940564f74bb0bded453c46a97033c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:18-ea-jdk-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:b7c285770680afce10a3812a1ab8d756dd02e5fb0626af1057f2ae0c60235295
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.7 MB (290678047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a901861d066e192607bf0f67c08598dbd0e130dbba7ee7d7c9d650ff022222c2`
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
# Wed, 09 Feb 2022 18:51:22 GMT
ENV JAVA_VERSION=18-ea+34
# Wed, 09 Feb 2022 18:51:53 GMT
COPY dir:570e617dc3556cc51d89cab6828d06005ee18874ddb9f3b36631503cd07a7d0d in C:\openjdk-18 
# Wed, 09 Feb 2022 18:52:06 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 09 Feb 2022 18:52:07 GMT
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
	-	`sha256:189b22cad28334fe5fb6166f274d39bf06e7d9e3d281901334e4d98d54b21ffd`  
		Last Modified: Wed, 09 Feb 2022 19:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526d35bac490ed7e2a6294232e02eb8810386e07f07e9d8108b734177fce4e67`  
		Last Modified: Wed, 09 Feb 2022 19:23:12 GMT  
		Size: 184.0 MB (183987155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794f232d07de5a04fee900db40bf0e5f415b9901702df428068317d842d6d143`  
		Last Modified: Wed, 09 Feb 2022 19:22:55 GMT  
		Size: 3.5 MB (3521722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266151f9d79c0ef850dcdbcb51a93a00633f8135c9ab9c08e5868e3a22aef005`  
		Last Modified: Wed, 09 Feb 2022 19:22:51 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
