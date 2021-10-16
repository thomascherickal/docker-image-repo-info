## `openjdk:17-nanoserver`

```console
$ docker pull openjdk@sha256:81e051d1950487d954f42efbb33de70404e555ed3802c8bad961924df6ef0b09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:17-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:1858d14daca58c7b0c50055eb7ae815051871917472d5726feac650b7a2bbe92
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.5 MB (288480183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdec7bed8e5891b1b503981e5367843115e6d96499f76898d06510d24606edd`
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
# Thu, 14 Oct 2021 00:45:54 GMT
ENV JAVA_VERSION=17
# Thu, 14 Oct 2021 00:46:11 GMT
COPY dir:16139fd5761a261a0505c9fb2561cbcbf9614d8d2403d5d2b56478bd7a396d2c in C:\openjdk-17 
# Thu, 14 Oct 2021 00:46:27 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 14 Oct 2021 00:46:27 GMT
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
	-	`sha256:315e62d363ed1350eb70d4fcab3e200bffc1503ffba162e44b115153b038243c`  
		Last Modified: Sat, 16 Oct 2021 00:41:19 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59bed6c822a7b9feba89be0b2643b3dce48e6dca6d4f59f889d2ae130f772e0`  
		Last Modified: Sat, 16 Oct 2021 00:41:38 GMT  
		Size: 182.1 MB (182093941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b26fe6df9c3084144794f8318a153cf5ba771c4fb2e7db88e254156aa559b2`  
		Last Modified: Sat, 16 Oct 2021 00:41:23 GMT  
		Size: 3.6 MB (3647912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5b49d1e8941b64e04ea2f48ac5d7c8df04f731ddec30922c33bc2c959d05c`  
		Last Modified: Sat, 16 Oct 2021 00:41:19 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
