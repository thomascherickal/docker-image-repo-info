## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:2d301e2e155010a5623b7897317edeaf7ca6bd27e471a3e9108f9d34b5d63641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:92791e170b622c93a8be5aa500e2f8a2582da9129307e1a09ea92d4611c36f60
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294728051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b52b052f0f6518b989e61f616b0f4b6bfac6548419cbfec31bc057108536c94`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 16:45:29 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 25 Aug 2021 16:45:30 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 25 Aug 2021 16:45:31 GMT
USER ContainerAdministrator
# Mon, 13 Sep 2021 18:29:31 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 13 Sep 2021 18:29:31 GMT
USER ContainerUser
# Mon, 13 Sep 2021 18:29:46 GMT
COPY dir:4c789b050c2a81313b7828df90f0ac6231d2beb7f7e21c1b81eca114d601d1fd in C:\openjdk-11 
# Mon, 13 Sep 2021 18:29:59 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 13 Sep 2021 18:30:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc7c72c6f1c474f2eb0355335032aadd0792a43c80c4000da20e8da5b268f5`  
		Last Modified: Wed, 25 Aug 2021 23:32:27 GMT  
		Size: 1.0 KB (1046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90849568386f9db56bd7ec7e79f509e2d38a892b209707162a5d056b6bb10f87`  
		Last Modified: Wed, 25 Aug 2021 23:32:27 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4006af65c1cc1c5d6267192e2de2ecaa8add3885e031061f1c6de62d9f8caf`  
		Last Modified: Wed, 25 Aug 2021 23:32:27 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456576eee5a9cbcddb59f7da7004a2d802c70d8f5855fae44ead92f654e04e39`  
		Last Modified: Mon, 13 Sep 2021 18:50:43 GMT  
		Size: 72.8 KB (72844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d171b2cf14b703f615a916d08244691e2e11256809434871ac80bc8735a7c608`  
		Last Modified: Mon, 13 Sep 2021 18:50:43 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd7370bbd747146d1a2bd32d87868e0f716f4511749e9dd3ec9e12bb3a9b60b`  
		Last Modified: Mon, 13 Sep 2021 18:54:14 GMT  
		Size: 191.9 MB (191857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28935b7cfcb986aa1a834db514980b7818f6fe7a494620afef82fe0c8e2162eb`  
		Last Modified: Mon, 13 Sep 2021 18:50:44 GMT  
		Size: 50.4 KB (50420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c6f084ca090a183b6c668281908bb80f6b6028dc434abd6032039c47654e9a`  
		Last Modified: Mon, 13 Sep 2021 18:50:43 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
