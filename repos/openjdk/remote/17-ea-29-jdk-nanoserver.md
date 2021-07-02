## `openjdk:17-ea-29-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:cd8f54752cfea7f35f4c079319cb831cf5fe7d857c580830866fc078e0bace7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:17-ea-29-jdk-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:bbdfa7ee3b387986d9a7383028d4fd3e65d559ada4df2076ab14de769ad485d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.5 MB (288470269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f536b12de5c53b88bee1a9e9b6f9463b325fd552841e249e1f380601b49e5f29`
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
# Fri, 02 Jul 2021 19:36:26 GMT
ENV JAVA_VERSION=17-ea+29
# Fri, 02 Jul 2021 19:36:43 GMT
COPY dir:dbb9caf38ccb2b51b8f82f6ee57b82955118d97367d555fcb04b5280a02280b3 in C:\openjdk-17 
# Fri, 02 Jul 2021 19:37:06 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 02 Jul 2021 19:37:08 GMT
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
	-	`sha256:9183f3ec0688b05e57fe5eb66565cf7e180459b926e58e0a400f20fc7a691741`  
		Last Modified: Fri, 02 Jul 2021 19:44:46 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943bf9ef5ca8129c31405767b5246537bc96498bfd6175a5889d8af333fb75ba`  
		Last Modified: Fri, 02 Jul 2021 19:45:05 GMT  
		Size: 182.1 MB (182075459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc16f12767e976d3ae0a0d1925e3beff7a8cfa586b98316d654066297e5950b`  
		Last Modified: Fri, 02 Jul 2021 19:44:47 GMT  
		Size: 3.6 MB (3646808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d878c00aac7cc4b68c980a22a706944a16479b55d58ff4ad29ec443182c8d9f`  
		Last Modified: Fri, 02 Jul 2021 19:44:46 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
