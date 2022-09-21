## `openjdk:20-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:a698a5c10de982fb267db7904ae7498498160e12290630ad0b17a84442ca390b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `openjdk:20-ea-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull openjdk@sha256:de703df3f3303a4dea88e1c98a4a50f8d57f60b735cb5a7482b297691697bcdf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (298993687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069d31776f5522ae1702359988b8d07b1c9a84970f1393458f2302394906de69`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 16:03:00 GMT
SHELL [cmd /s /c]
# Wed, 14 Sep 2022 17:08:57 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Sep 2022 17:08:57 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 17:09:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Sep 2022 17:09:07 GMT
USER ContainerUser
# Tue, 20 Sep 2022 23:19:56 GMT
ENV JAVA_VERSION=20-ea+15
# Tue, 20 Sep 2022 23:20:11 GMT
COPY dir:87dd871a3a021bd29beb753adab165af4a8a2fce95fec627f04c9f7096c13386 in C:\openjdk-20 
# Tue, 20 Sep 2022 23:20:29 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Tue, 20 Sep 2022 23:20:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:233f09b2a52487084f2cfb5e06dac2815651432c9d37c729582f59cfcf66b243`  
		Last Modified: Wed, 14 Sep 2022 16:47:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f67cb607010c6768708866762c8f245af049da7669af90242ea7dc3d1881f80`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd0c7e3fefcb9d81347f1ab494f4177ae8fff7d71ac827f5e90d34ee4bf483`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72046412150cabb4b6b5ba4cf56188800073ddce5f570b7d921bc62eb13c577`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 67.8 KB (67836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea99aee812db540f38ee961b7634ec0afe7d8468d85e3adaabe234fee1414d5`  
		Last Modified: Wed, 14 Sep 2022 17:22:51 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f1244949e8c98f381be06b961a5cf51ae26d3ddbb42626e265cd62b8bc643d`  
		Last Modified: Wed, 21 Sep 2022 00:19:05 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5f8fedfa7535670f36027bdd65be6bdda1e32b16fb83e4931b11fb0c351e44`  
		Last Modified: Wed, 21 Sep 2022 00:19:26 GMT  
		Size: 191.8 MB (191837676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3591c0f2359f4cd36318921de7d297221ef4e4b9514c777411e843cd82e70b8b`  
		Last Modified: Wed, 21 Sep 2022 00:19:06 GMT  
		Size: 3.7 MB (3747176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c49f8c11805c4255de29b270c760b0faeb33b8ee1d18f3546db348112d0a792`  
		Last Modified: Wed, 21 Sep 2022 00:19:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
