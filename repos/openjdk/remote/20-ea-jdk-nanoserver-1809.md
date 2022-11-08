## `openjdk:20-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:fdfc71d0fce793f31ae89b62dc8c1b4f918d42143e48831162cd644183c718ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-jdk-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:bb7de609b3e8d4e7e88ae5e7850fe62a65403acf0a063b133b3c4c29af0bae24
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303844476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef988e245cefd3f6b38136303fda63bfb670c400cdf1356614e4f2ef3a7292a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 15:20:49 GMT
SHELL [cmd /s /c]
# Wed, 12 Oct 2022 16:43:51 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:43:51 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 16:44:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 Oct 2022 16:44:03 GMT
USER ContainerUser
# Mon, 07 Nov 2022 21:19:44 GMT
ENV JAVA_VERSION=20-ea+22
# Mon, 07 Nov 2022 21:20:01 GMT
COPY dir:aad69aed6f652d82aa51467e9aa3388f27a3c781e2cc620a3dc458bdb415983c in C:\openjdk-20 
# Mon, 07 Nov 2022 21:20:28 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 07 Nov 2022 21:20:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a667d76c19fca171390d60fb90c40e16c777050e943a7fe17ad7686841f0f`  
		Last Modified: Wed, 12 Oct 2022 16:02:59 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4315d417eb7958a05c7977d0ea6b1b4745e46725d02f23235173bbad2c73101d`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c783713d738fc9dfff161ad3ff4369333cd0881466ab886feb09e6ef3508512e`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05686fefb2145f84031cd9cae616dd90496d078df87f19c080931972eb700e7c`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 67.2 KB (67186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab8462cae193737dba91e48900abf79d1b7234b48f337497ae0abfe9d8189e5`  
		Last Modified: Wed, 12 Oct 2022 16:53:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd3eff485b12ba84cf008037019b637cfb1bb4fb6a5ffddce575e8d7b9119a9`  
		Last Modified: Mon, 07 Nov 2022 23:19:53 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ccf3707ac33a7c0a704695ecb2178f5f066cba1303c6dbb4add38d264eb44`  
		Last Modified: Mon, 07 Nov 2022 23:20:14 GMT  
		Size: 193.2 MB (193207341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2676512fdece053aa02707ca214fee04cdae618496b11c0f0f45bc20d7e84773`  
		Last Modified: Mon, 07 Nov 2022 23:19:54 GMT  
		Size: 3.8 MB (3789241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219e60541f25fd0f64cbe1afdc000d7ceed7cd21c72a26eef8de88b9047c11a5`  
		Last Modified: Mon, 07 Nov 2022 23:19:53 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
