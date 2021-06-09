## `openjdk:17-ea-25-nanoserver-1809`

```console
$ docker pull openjdk@sha256:7a139c12ae67cedc196a822350c0c6d7f660a280dc3cadb9c7cbab35736c6e1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:17-ea-25-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:c45760b3c731e1d4110896358c61967861d722b4716ee82f29cfd20f95b37426
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.4 MB (287376327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872006717fb0bef025815b998afde62cbc277fcbf7c9530528f23e39c11dbd5d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 16:52:42 GMT
SHELL [cmd /s /c]
# Wed, 09 Jun 2021 16:52:44 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 09 Jun 2021 16:52:46 GMT
USER ContainerAdministrator
# Wed, 09 Jun 2021 16:53:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Jun 2021 16:53:09 GMT
USER ContainerUser
# Wed, 09 Jun 2021 16:53:11 GMT
ENV JAVA_VERSION=17-ea+25
# Wed, 09 Jun 2021 16:53:29 GMT
COPY dir:2cba33c1c102797dc756ff46d5def95468416517112f1eba2a9b024090e94db0 in C:\openjdk-17 
# Wed, 09 Jun 2021 16:53:53 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 09 Jun 2021 16:53:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:acc28506464ab4d21eaffeb562876f3408463a46d298d12ded7ac0e3dd3c1bd6`  
		Last Modified: Wed, 09 Jun 2021 17:25:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a017ad6d2c865b2b606d1d084d50c43233147ea5cf53857802c790c6c01b7c3`  
		Last Modified: Wed, 09 Jun 2021 17:25:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3e213028246803502d07da137fca93406b7b31a282ab02ef95a4e7547b1e1`  
		Last Modified: Wed, 09 Jun 2021 17:25:26 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24145c50d278aaa44ac5a4bc31c1b03bac6fcd0d7e2d291c01685bc9b4260369`  
		Last Modified: Wed, 09 Jun 2021 17:25:26 GMT  
		Size: 69.6 KB (69634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0442665d8729ebbf2ff71dbd067a8b13f6af08edd7d070d9ba24a2e9e30285f8`  
		Last Modified: Wed, 09 Jun 2021 17:25:24 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ca159d91d3b25b755620e85c12645437bb36d27af760059e0ac1aeea510bc2`  
		Last Modified: Wed, 09 Jun 2021 17:25:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57531d80034b2fcbe83d651f62139df0bc886a7ea4d90b00a83176dabe9cd1b6`  
		Last Modified: Wed, 09 Jun 2021 17:25:44 GMT  
		Size: 181.0 MB (180988574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86fa0a325ee9f7dff92eb483161f33820bb62596586eaf6016ef2b51f743bd4`  
		Last Modified: Wed, 09 Jun 2021 17:25:25 GMT  
		Size: 3.6 MB (3639809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea20f28d3485b93e81ac232ece36b64b89deeecc8057be8dfe968e67243ec9`  
		Last Modified: Wed, 09 Jun 2021 17:25:23 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
