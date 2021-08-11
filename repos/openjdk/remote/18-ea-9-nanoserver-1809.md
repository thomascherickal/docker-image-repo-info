## `openjdk:18-ea-9-nanoserver-1809`

```console
$ docker pull openjdk@sha256:aaf5c2c4ae2d4edc22da81bceb12ce8c3ec8936f896c8652f4dd6c4e304986db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:18-ea-9-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:fa6b73025514883a3c00f9b91eba312a884ff1eba29317f1f25c8e1c46073c72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289105777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69996fcd4cd33eb1aedceba0a5af68ae4e687ab6e3f0b3860b05b05828d659c0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 17:30:38 GMT
SHELL [cmd /s /c]
# Wed, 11 Aug 2021 17:30:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 Aug 2021 17:30:43 GMT
USER ContainerAdministrator
# Wed, 11 Aug 2021 17:31:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 Aug 2021 17:31:09 GMT
USER ContainerUser
# Wed, 11 Aug 2021 17:31:11 GMT
ENV JAVA_VERSION=18-ea+9
# Wed, 11 Aug 2021 17:31:31 GMT
COPY dir:90ec8134647146eac9e668dce7afdccf7a2a64d110862971c025e25f054d7a45 in C:\openjdk-18 
# Wed, 11 Aug 2021 17:31:53 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 11 Aug 2021 17:31:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae0a5a946be2ad0e39a8260e454c0060a31a9f7e5be75d1f9038dc13730abc0a`  
		Last Modified: Wed, 11 Aug 2021 18:21:28 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3e3ce6f906341a31b594d25772e87453477f92df500f7e55c033ee65d1f7b8`  
		Last Modified: Wed, 11 Aug 2021 18:21:27 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4140a377a80813839c51929577daa32b3f49ead3975b3b71a2106af7999f7c`  
		Last Modified: Wed, 11 Aug 2021 18:21:28 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeec1a666d3ea4495353e16515d8a87648b15d6c51c137b53bfba178aa5a36b`  
		Last Modified: Wed, 11 Aug 2021 18:21:27 GMT  
		Size: 68.6 KB (68571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bce606c6fc4ebc45e038cdeefb933ddc75feed60a9793ef5682fcacbeb615c`  
		Last Modified: Wed, 11 Aug 2021 18:21:24 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826b88ff3e19e0ff241fe284267a59c9bb39aaebd9a0a8404d09ac83fff9cf76`  
		Last Modified: Wed, 11 Aug 2021 18:21:24 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac292061ca58bd658163e0b92beffa56fc2e8dad48142639809fd10f0caa455`  
		Last Modified: Wed, 11 Aug 2021 18:21:44 GMT  
		Size: 182.7 MB (182675304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98be9e8f3a56126596402db142ef0fba09c0766110828878dbb9cb7604cee25`  
		Last Modified: Wed, 11 Aug 2021 18:21:25 GMT  
		Size: 3.6 MB (3613816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7926e27a88ab044bcf260327e465850c963266af777be3fef6df55349ce1b9b4`  
		Last Modified: Wed, 11 Aug 2021 18:21:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
