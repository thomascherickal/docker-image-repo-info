## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:ce2e38e3c87dbe28e36e8ce48dd7a07a5a0f4de4a9251db48c88b6291de506bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:863af53153f72f1c67717a8fd077463c7aa348f4a4bf74bfb838972863e4e527
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141650834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adae14b8e4d08aed430841e200dcc4d48251ab1c6a0ac14147b98a1ff063f2d3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:21:14 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Aug 2022 17:21:15 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:21:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:21:25 GMT
USER ContainerUser
# Wed, 10 Aug 2022 17:21:25 GMT
ENV JAVA_VERSION=8u342
# Wed, 10 Aug 2022 17:23:53 GMT
COPY dir:d5a496d08a96fa54c304808d847f638574e6a63a370788ac54376505e1387a54 in C:\openjdk-8 
# Wed, 10 Aug 2022 17:24:04 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6f03744b411c834fff8541b86c417dd9cebbbfd149ea75944e3d1c8766aa8e`  
		Last Modified: Wed, 10 Aug 2022 17:37:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e306e6fe26dd8faac775af256f32982b10533d20c3781942b4e464ea13493b`  
		Last Modified: Wed, 10 Aug 2022 17:37:32 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d005dbf9dda3bf691f799d207ea911cf138f23df57a88ec12b25dd874ad854`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 67.6 KB (67569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e58525a260d7308aeb21e49035b7588309aae8b4fe37c17563ea45ba947028`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ba3f94dcb65edc82c61f421dc102e7dfd352a8a761de9992c40fdb23dc3018`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19faf5493759bec9630b559dfef50ac1b0d708eed3500c3369432bc2d39ad3e`  
		Last Modified: Wed, 10 Aug 2022 17:38:32 GMT  
		Size: 38.3 MB (38291870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59048e6d6c5c0cab1ab26040be0fc8addb9bb23f26771881a9f1fbac1cec980`  
		Last Modified: Wed, 10 Aug 2022 17:38:27 GMT  
		Size: 81.4 KB (81429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
