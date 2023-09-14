## `openjdk:22-ea-15-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:9f5ee59c062acc849335c64f55124bf76659d13a816bfac680966f6f1284127a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `openjdk:22-ea-15-jdk-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull openjdk@sha256:abae2f7ab71b771ea48224a8e748ff1c34ad8d2925567c2e4e25f2ba53aeb858
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.5 MB (307511433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e8544577355959e7775502dfd1c1107d42bd7614aff1b27e253d0c80534dec`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 02:29:44 GMT
SHELL [cmd /s /c]
# Wed, 13 Sep 2023 05:19:19 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Sep 2023 05:19:19 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 05:19:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Sep 2023 05:19:25 GMT
USER ContainerUser
# Thu, 14 Sep 2023 22:33:34 GMT
ENV JAVA_VERSION=22-ea+15
# Thu, 14 Sep 2023 22:33:48 GMT
COPY dir:ce12bd8ea9fd472a769e3c8a450fa705d2b5e09a2344de1856cd63030dff1bd4 in C:\openjdk-22 
# Thu, 14 Sep 2023 22:33:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 14 Sep 2023 22:33:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a5bcbc9b0f0398bf8f14c235b24ba85d9acacf855518119cd1ce338a235a15`  
		Last Modified: Wed, 13 Sep 2023 03:36:33 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6f344751fdeca77c774720f1f5845e2a683d1ed1b251bd6e554f91ab03d2b0`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be8c52d7c546ce325f7f3606c55b22e94fd1925aba26440028f33d2a873ff1`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de794e4f653951d19d788489e6c197cbbaa2864a36a169d068b25cf13ea0c6a6`  
		Last Modified: Wed, 13 Sep 2023 05:26:46 GMT  
		Size: 79.5 KB (79476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4673df9416ca713de65ecb18e35ecfcad8bafedd6b1e61dca148de841d138b7`  
		Last Modified: Wed, 13 Sep 2023 05:26:44 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f1789e84601c2ab85e5472966d760be3a37ae4bb31990df52386b71c6c417`  
		Last Modified: Thu, 14 Sep 2023 22:36:40 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1682cb4d02998be36af7c47b768acc9761bbc064e00a9c0d13390eb94b1cb2e`  
		Last Modified: Thu, 14 Sep 2023 22:36:59 GMT  
		Size: 199.1 MB (199118669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a391bb3696dea9fecdb77760ef65456599fab27b5aa63fceeabd9448342bf5fe`  
		Last Modified: Thu, 14 Sep 2023 22:36:41 GMT  
		Size: 3.8 MB (3813860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1b7bb0df049a80a6e54873817240185c1f487b6780a730d5f534b29040e7a`  
		Last Modified: Thu, 14 Sep 2023 22:36:40 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
