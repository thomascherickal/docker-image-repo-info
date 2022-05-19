## `openjdk:nanoserver`

```console
$ docker pull openjdk@sha256:dca87d2a7712c219495470fc5716606a754436a51064434a4d4236f411fc2989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:109183b13f510e3ff077618edd7da0bf0dcb55b28f4cda0d81684a04ae8028fa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289477151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd2670ec84321a6f89e33c5894a748c29884c8d8456ef07a915f1e19c4b6b3e8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:10:18 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Apr 2022 17:10:18 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:10:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:10:24 GMT
USER ContainerUser
# Wed, 13 Apr 2022 17:10:25 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 13 Apr 2022 17:10:39 GMT
COPY dir:09e6dae9f6621f372798a539a0041951600f85effa47175a1c021c5940e0e226 in C:\openjdk-17 
# Wed, 13 Apr 2022 17:10:51 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 13 Apr 2022 17:10:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b9fc6b9b208737e6371780703c3bc0f91ded2751ef412860d2c8f4c48153bb`  
		Last Modified: Tue, 19 Apr 2022 01:03:28 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd048f810e4e2d7b297572a8f0efeeb1973c332c5321a2df7884ab144b8878e`  
		Last Modified: Tue, 19 Apr 2022 01:03:28 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f60d551a8c256e38f6bcdb5493723153eb432ad013bd996c59b62e88623173`  
		Last Modified: Tue, 19 Apr 2022 01:03:28 GMT  
		Size: 68.0 KB (68041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ca84694dddadf3554151879c9e24d077fe62b36fc10de47aea8317d565d4c1`  
		Last Modified: Tue, 19 Apr 2022 01:03:26 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c58c8df86383244ee53103cdf0ccb6906bd4d4106c8cb08f2a3fd206aa6ac34`  
		Last Modified: Tue, 19 Apr 2022 01:03:26 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245125db6995f98eda970c99863044ac2daaf574122e3acb3f6174052ecb7a15`  
		Last Modified: Tue, 19 Apr 2022 01:06:33 GMT  
		Size: 182.6 MB (182614650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84156ab53a3729db7cd8597086e4ed30b638570bb4d43e2755783d3ebb8c10ca`  
		Last Modified: Tue, 19 Apr 2022 01:03:30 GMT  
		Size: 3.7 MB (3691526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa98f1284c955b846da3bf0b4fdcfcea8deda52349045a6a4856a5034216ef51`  
		Last Modified: Tue, 19 Apr 2022 01:03:26 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
