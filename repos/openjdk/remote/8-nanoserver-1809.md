## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5391b29f5ea6ec24f77f92e39bf56bea1783f1603ed91fe8d22b5eb9949b0aa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:05ca4aed0a28081aa78edc7196bc914248f24416a8a1683a13e7cbdfc0881124
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.3 MB (204261717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a187e6e1c9a49ffc659397e52f6cabd9c45929f3992b69691f7e70c9c0db509`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 16:14:00 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Jul 2022 16:14:01 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 16:14:12 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 16:14:13 GMT
USER ContainerUser
# Mon, 25 Jul 2022 20:26:36 GMT
ENV JAVA_VERSION=8u342
# Mon, 25 Jul 2022 20:26:52 GMT
COPY dir:9c3bba9710713dbb55751ce63d59239c9d60548d5128ebf71c30f559bc754473 in C:\openjdk-8 
# Mon, 25 Jul 2022 20:27:15 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148f24fdace3fb9dfc469abd587650fafdf6306095591fbac5f681ea330560c0`  
		Last Modified: Mon, 18 Jul 2022 21:32:02 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f93316072971a85b9949521e5e6ecf59d21bdc3581fc1e1add713febb868ef0`  
		Last Modified: Mon, 18 Jul 2022 21:32:02 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed149726e806a0166236d15cf4fc5ea65eb1da4033351d46fa58aa3f704aa85`  
		Last Modified: Mon, 18 Jul 2022 21:31:59 GMT  
		Size: 72.7 KB (72654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fcf0621e58eee5b24877bc6f1542450faf983b06d868581b56b39dc69597f3`  
		Last Modified: Mon, 18 Jul 2022 21:31:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bede253169cd0a4f89cc3b4f8d1608819886a4284bb0c7ec1edadc23386be2`  
		Last Modified: Mon, 25 Jul 2022 20:37:21 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622feec13545fc20807b7ae06bb578a1be97deb0fb8467b2ab7f8bc5263ced99`  
		Last Modified: Mon, 25 Jul 2022 20:37:34 GMT  
		Size: 101.0 MB (100963070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db600f37b9d51ee7ed30d5403623f61af5cd6b07ce0c4aabdaf98d497911dbf`  
		Last Modified: Mon, 25 Jul 2022 20:37:21 GMT  
		Size: 65.3 KB (65261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
