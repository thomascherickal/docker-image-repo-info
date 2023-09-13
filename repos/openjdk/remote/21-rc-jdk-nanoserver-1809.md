## `openjdk:21-rc-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:36b250a74706da1b4f5bc134cd242b1a98d8c92ea2825a2f0810ffe97f821cb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `openjdk:21-rc-jdk-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull openjdk@sha256:dde1e6be93c991282816790e711a7c105e78e81f5eb018a17d2403bdd9e3d58c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.4 MB (306432884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806bf28fea820ebe58395b6cac3965788484ba7702a93ea470106c4a6d7d7f58`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 02:29:44 GMT
SHELL [cmd /s /c]
# Wed, 13 Sep 2023 05:24:07 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 13 Sep 2023 05:24:08 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 05:24:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Sep 2023 05:24:14 GMT
USER ContainerUser
# Wed, 13 Sep 2023 05:24:14 GMT
ENV JAVA_VERSION=21
# Wed, 13 Sep 2023 05:24:28 GMT
COPY dir:ab44a5695be5306db50e482755419b90c734a5e54efb6807b2ffc8de111bd777 in C:\openjdk-21 
# Wed, 13 Sep 2023 05:24:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 13 Sep 2023 05:24:39 GMT
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
	-	`sha256:80c9e49ecff3d3fec81f8baba72bd178d3ffe63a79ec703c6448e57ed4e0f390`  
		Last Modified: Wed, 13 Sep 2023 05:28:30 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09072ef743f9380ee862018b80938caa988196cb6a1b5c5982a93825956493c6`  
		Last Modified: Wed, 13 Sep 2023 05:28:30 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8211d7647eb4b06764f997ad0ad83cfbc16f9d2cec34b4a1478aecbcaa8b78`  
		Last Modified: Wed, 13 Sep 2023 05:28:30 GMT  
		Size: 69.3 KB (69271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564c4f6a80e4c03661d4aef252a6cd6ecb9f5c647791b99ed9ca4bba4fd98029`  
		Last Modified: Wed, 13 Sep 2023 05:28:28 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95bbecae930772bb7e6504e5af8c16ec8efac3388808032d46525044173e119`  
		Last Modified: Wed, 13 Sep 2023 05:28:28 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bb72ab74f92572260a4c5ed7a40e9d5b0273a72b4c364f63592cbbe96a3b5`  
		Last Modified: Wed, 13 Sep 2023 05:28:47 GMT  
		Size: 198.0 MB (198039960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea0594e4218c21b6769b0bef42b290359ccd9b2a3b239e5d9f5dbf7964ca8b`  
		Last Modified: Wed, 13 Sep 2023 05:28:29 GMT  
		Size: 3.8 MB (3824291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362e1b2786865f3e09f71d5d1303d32dd6f0c622dd67c5b35e358039a26507aa`  
		Last Modified: Wed, 13 Sep 2023 05:28:28 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
