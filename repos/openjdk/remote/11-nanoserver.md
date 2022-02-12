## `openjdk:11-nanoserver`

```console
$ docker pull openjdk@sha256:3684c9ce0e7daa56535cc31ff8d47c74fc898b5718f89f2ab738bed36a4c6caa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:11-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:eb268543f13dae98bc50d4f5dcba1005ca78e7f4732735be811fee2fbf980db4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292519716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:387415ad73a4711ae37fbdb8a238c61ffdea6642ffcc54bf007c6a4e8f688a6b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 19:02:37 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 09 Feb 2022 19:02:38 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 19:02:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 19:02:48 GMT
USER ContainerUser
# Fri, 11 Feb 2022 23:28:11 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:28:44 GMT
COPY dir:0759968b5468f4f347700ffdc4419593add6654a39f7928925a20866474eedc9 in C:\openjdk-11 
# Fri, 11 Feb 2022 23:28:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 11 Feb 2022 23:28:58 GMT
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
	-	`sha256:3ac0bf48a54e2421f92f124b47d38ee9ad764043cc5f5cb52e8f8ba04f00ce99`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623100c5e8a6de92e548ce8bc6390263e442d776c8437eccc5827c051c65826`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa70386997aa574dc9d8458d26c8e3871a3c8389b44b3b39c60ecf4a08278b5`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 70.6 KB (70555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6524283bfbd3d6b592d22322ad58960ceaa05bd51127df706da1032f4f9d0188`  
		Last Modified: Wed, 09 Feb 2022 19:30:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aad9169f5a71e1f7e6abec542e191e8df474eba027b6e447b971c639ce51624`  
		Last Modified: Fri, 11 Feb 2022 23:51:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7b21d7e35367caffd3e56d15a16f6b887b9d49cd0bedf0160ea40c3dcbd5e`  
		Last Modified: Fri, 11 Feb 2022 23:51:44 GMT  
		Size: 189.3 MB (189298518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2894e9c37375829b767591a5ff07421026059550d61383777ffd82d7bfd34047`  
		Last Modified: Fri, 11 Feb 2022 23:51:25 GMT  
		Size: 56.6 KB (56615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5901100c68f048e358ef386504cc10eafca464b565f0291310473b0a2dd175b8`  
		Last Modified: Fri, 11 Feb 2022 23:51:25 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
