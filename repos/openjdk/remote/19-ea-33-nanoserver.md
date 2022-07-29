## `openjdk:19-ea-33-nanoserver`

```console
$ docker pull openjdk@sha256:46b5fe3a013af2493abbd86700574496fc2b40ad735892a2e6bff9c90a2b80c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:19-ea-33-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:823232a260cfd159992173ec06cd193e826c388c4b6ac57e8d67ef575478f678
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.1 MB (298147987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806540096ed15c8242c158fe76f95094d27f279228a8051a17695758ca73fcf7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:57:38 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:57:39 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:57:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 15:57:47 GMT
USER ContainerUser
# Fri, 29 Jul 2022 01:23:04 GMT
ENV JAVA_VERSION=19-ea+33
# Fri, 29 Jul 2022 01:23:19 GMT
COPY dir:a469ca94c633927b92029b3300922afd77da10af7540c7299efb65e8a1b0e3d3 in C:\openjdk-19 
# Fri, 29 Jul 2022 01:23:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 29 Jul 2022 01:23:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24a8dc780930fe59a9967fb76b10b2fb2ac36ff76c3697586a3df823f25ab8d`  
		Last Modified: Mon, 18 Jul 2022 21:24:44 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1582b9bf63a2d6ede0a45ecb506c093cf9a09b81e8de25dd46c5bffa9c7d94`  
		Last Modified: Mon, 18 Jul 2022 21:24:43 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4239363179c317c462b5006da97ce6faa8c7e4256719a99f4c3dd0cb7a4b524f`  
		Last Modified: Mon, 18 Jul 2022 21:24:43 GMT  
		Size: 69.0 KB (69030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dd52e79d9b5ebce7877fd3f3e42eb3c3cfae509d375aa166c3a01cb8e29a9`  
		Last Modified: Mon, 18 Jul 2022 21:24:41 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6171199947be044ebe713781441cb48e09861a8f9e32006fe4fced20769a1fc5`  
		Last Modified: Fri, 29 Jul 2022 03:23:16 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44721c880c64e655f2e4b69d996125e31f553049bbaa15e89dac9704f9d8d7c2`  
		Last Modified: Fri, 29 Jul 2022 03:23:39 GMT  
		Size: 191.2 MB (191198933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449227b14191c769a5966b4f99315b625d259dbaeeee2050395b272f0831faf7`  
		Last Modified: Fri, 29 Jul 2022 03:23:18 GMT  
		Size: 3.7 MB (3718414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913cb59bbb582c629b2ad17ebdcb0c0cc25cc3dc6aeb4da456b134dc4b690fa6`  
		Last Modified: Fri, 29 Jul 2022 03:23:16 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
