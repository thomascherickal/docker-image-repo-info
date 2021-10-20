## `openjdk:nanoserver-1809`

```console
$ docker pull openjdk@sha256:055c3c4966a4b42904ce03563b490810d1549597f81e019a83e290d6dd87d3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:bf4452160b83e757997ab07e748fc22232884db7318b3cf8b1e87524a9e1443f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.5 MB (288509142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0333fc53737f2d32de5fc6add4b855c8c8966e54699d55bcba28361490dd4df5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 00:45:42 GMT
ENV JAVA_HOME=C:\openjdk-17
# Thu, 14 Oct 2021 00:45:42 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 00:45:52 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 00:45:53 GMT
USER ContainerUser
# Tue, 19 Oct 2021 22:18:56 GMT
ENV JAVA_VERSION=17.0.1
# Tue, 19 Oct 2021 22:19:13 GMT
COPY dir:e704eeaa3bdd5594ba06b91011a1085b7cda6db494a4c160caef3f39aec0ac18 in C:\openjdk-17 
# Tue, 19 Oct 2021 22:19:40 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Tue, 19 Oct 2021 22:19:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87f72d6af0be4c3ec201f5540287b5311dfca49e967782ad06942116f57e691`  
		Last Modified: Sat, 16 Oct 2021 00:41:21 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ddff790b9affbcc1fbffc139ee5ebebd723561ebf598454b597731564ffa7a`  
		Last Modified: Sat, 16 Oct 2021 00:41:21 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1307b921aafabeb366dbbf5689271289bc3bd8eb55248752632648f4eb0232a`  
		Last Modified: Sat, 16 Oct 2021 00:41:21 GMT  
		Size: 70.2 KB (70220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bddaa9b47bbaa5f77a4666c9fee38db21b9ab1f6885d504ff1231c9cdec4ec`  
		Last Modified: Sat, 16 Oct 2021 00:41:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44141711609b5f04d0d5559209b26aabdb9734f5f8c06be07769af599afcd7b2`  
		Last Modified: Tue, 19 Oct 2021 23:24:42 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769dab0bfcbbae14019cfaefffe0b25b8a7710a49dee4b0580a6d2c631f4b470`  
		Last Modified: Tue, 19 Oct 2021 23:25:02 GMT  
		Size: 182.1 MB (182120251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d4c80f7fabb79a43f8db8c645a0e81697cfc5177a09a3771e605d18c5e4382`  
		Last Modified: Tue, 19 Oct 2021 23:24:46 GMT  
		Size: 3.7 MB (3650500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1066615bcf6d575a8ef14af98f2fc4745b17adfa142dca559108930ac8f40c`  
		Last Modified: Tue, 19 Oct 2021 23:24:42 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
