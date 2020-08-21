## `openjdk:16-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:98360a0d604060a8fa181fb5166fcfbf96fc3bf0e0926540df2f995facf36985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:16-ea-jdk-nanoserver` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:9666b0e779b792143259312e2de76665e67fc69f4c67dcc8db78b1748a7701c1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.8 MB (296784204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3449009dbcf1c656a1fac41ffabe21d7929a888baecf07275c97d7a66dbd7a3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:28:05 GMT
SHELL [cmd /s /c]
# Wed, 12 Aug 2020 15:28:06 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 12 Aug 2020 15:28:06 GMT
USER ContainerAdministrator
# Wed, 12 Aug 2020 15:28:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 12 Aug 2020 15:28:22 GMT
USER ContainerUser
# Fri, 21 Aug 2020 21:19:53 GMT
ENV JAVA_VERSION=16-ea+12
# Fri, 21 Aug 2020 21:20:32 GMT
COPY dir:d1253d3bcc8f61a4ec0d0c7f3b1eeece6d2e72a28048a6220c5743b09f5dde91 in C:\openjdk-16 
# Fri, 21 Aug 2020 21:20:59 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 21 Aug 2020 21:21:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1c7c341c7a3d0c7b6e849b6faec560815682d07ce87df2e4d1e83f928aab306b`  
		Last Modified: Wed, 12 Aug 2020 16:10:21 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ff90b84cb0e951da0f399342768862ac8c294fbe71e80d787a60d9cc2c7b5`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566429948e6233b746b6d219e57703486a6f2f00910b8e1842ff9920d1834e1`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4bcc2b175dfe1adf68a872a4fa40033320f09b67b59f3dbf35cae4783189d4`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 65.9 KB (65918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca4105c8d6a5159a2ffd6904f118076cb11506891820a04656978435fd29bad`  
		Last Modified: Wed, 12 Aug 2020 16:10:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e73fd2614c11d5316bc38df5d99dca0160a97f6459e71f6b5952a94057ef4b`  
		Last Modified: Fri, 21 Aug 2020 21:26:15 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ea62b0603afa898e144251fbb44a96d477e7ded14bff345906eaf9b719fe91`  
		Last Modified: Fri, 21 Aug 2020 21:26:34 GMT  
		Size: 192.2 MB (192209579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631fedb0f3dec9a0fe1743ba4ea3e1e59296f36aedfbceef41f7b5479f33b73f`  
		Last Modified: Fri, 21 Aug 2020 21:26:16 GMT  
		Size: 3.5 MB (3518500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956d6fe09af67341f56d1fbd31435a6732545a98b6bdceecc3dd3475cb3fe170`  
		Last Modified: Fri, 21 Aug 2020 21:26:15 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
