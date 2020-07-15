## `openjdk:16-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:aa924f675e7c325407f138971dbddd92efdfe17a22b8957005412ee9d991e50a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:16-ea-jdk-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:df8eefd5f6c86299d69ed6fd60ab056d6476dbf772695d96217505d8e8e8549e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.5 MB (296466740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f0bc1bc0984623f3429a862707a991175de4565c3a7895717e511a2dc37cd1c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 01:54:44 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:54:45 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 01:55:00 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 01:55:01 GMT
USER ContainerUser
# Wed, 15 Jul 2020 01:55:02 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 15 Jul 2020 01:55:55 GMT
COPY dir:ab91ee3bf26eda34a581e70062adc4a24889abc64f935e4fe64edf4b7fd621b4 in C:\openjdk-16 
# Wed, 15 Jul 2020 01:56:16 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 15 Jul 2020 01:56:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952f154db0b1aa57586a649f933acc22620a18dc11bfe0f2369af17af77fd616`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d574471402fee7c0d2fb574eb4bbfd848f720c971dc4d9318a7437da54d1ee`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3532803eda54cf6b27e5f89a60ea866a566b1e68dc2a18b9e108adc19b202d0`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 65.7 KB (65688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96519e5bd9ea0e996eef2754f2ea5fdffd216464dc67d36374e07735cd0134fc`  
		Last Modified: Wed, 15 Jul 2020 02:43:52 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866bc6b574097d8bae577b02eb545f963938ddb4550464ecd3c76a00cb0d4e70`  
		Last Modified: Wed, 15 Jul 2020 02:43:52 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c5ab1052b32aac347067ae45531c124d2f3c07460c76b809dfce0f8683968`  
		Last Modified: Wed, 15 Jul 2020 02:44:13 GMT  
		Size: 192.0 MB (191970749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6ada4edff86cdba799018d0c555b8ed8e6dec7f0672b1039ec276b25ab5a5b`  
		Last Modified: Wed, 15 Jul 2020 02:43:53 GMT  
		Size: 3.5 MB (3529443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55ae9c714d525daadd2ce8071fc28469168433f1a13b81ca618dab675a7a63c`  
		Last Modified: Wed, 15 Jul 2020 02:43:52 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
