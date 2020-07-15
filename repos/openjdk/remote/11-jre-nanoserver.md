## `openjdk:11-jre-nanoserver`

```console
$ docker pull openjdk@sha256:ec7e322fa81d0336deabce51652f7504dd292e2522a68c9b02aa6a85a5482d83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:11-jre-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:b45117087ab76eb0db353c7574e0a04a278a959e901e96e2fdb9c0419ca6d3fb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.2 MB (140161631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7cab7297b2da38ae7e496a514fc8b3b308e907694716b2d8c7701f363eb9387`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:21:21 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Jul 2020 02:21:22 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 02:21:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 02:21:34 GMT
USER ContainerUser
# Wed, 15 Jul 2020 02:21:35 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 15 Jul 2020 02:27:10 GMT
COPY dir:5079dca1201fb18611f476ef87596f1f7b8bce8e365c08f25921689ee5b44ccb in C:\openjdk-11 
# Wed, 15 Jul 2020 02:27:25 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edf2cf232929022745a17a752c11091206fd6804fbcd0deb0cf94f65d838e43`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34289060bcecad92a4781d988ddd844d829452e51a1c73c3f2608a0a6085c77`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78522c618af5554ffd3adf8623d7933e1792428e86ad573127cee6fdc3a590d`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 64.2 KB (64206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608ac22c3f2ef90c8c5bc20a0fe2c584d51c075fe6bf2a5b7509df4c32d755d`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5471947ff5dafa77f1d05926afd2d7caaa25c826f05f5cf8a6dc597d83777`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504dba6817973f97b5a4c0ec6375018bb40ccfbc1b30786f86a0a14d3315b179`  
		Last Modified: Wed, 15 Jul 2020 02:53:15 GMT  
		Size: 39.1 MB (39121378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbe0d33b79b29094de7476fc7e2ee9a973d6e84a1012452dfc8a2b98d540f`  
		Last Modified: Wed, 15 Jul 2020 02:53:07 GMT  
		Size: 76.0 KB (75966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
