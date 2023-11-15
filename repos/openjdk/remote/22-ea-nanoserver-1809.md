## `openjdk:22-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:ea878400cafd0787f4da72852146c2603181e6f90e7a41d2690e83ef83065c42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-ea-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:05252f04716a6168bb31ee6ad7e6c5f00dcadc1a08d0c1419bd58b87e352cd54
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.4 MB (308382640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703b9731ff93422b7c201a523e6810ac0ef7b6c5695e2ab2843676691b0ca6b2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 03:54:23 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 11 Oct 2023 03:54:24 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 03:54:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 Oct 2023 03:54:36 GMT
USER ContainerUser
# Wed, 15 Nov 2023 03:46:00 GMT
ENV JAVA_VERSION=22-ea+23
# Wed, 15 Nov 2023 03:46:17 GMT
COPY dir:7a47213a9d830d9c4246c0f1198f6179f788435f5144076c8867ff083c4a5bcd in C:\openjdk-22 
# Wed, 15 Nov 2023 03:46:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 15 Nov 2023 03:46:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f7d94044a293783b6667a23790497e452737d17d7221e9fcf940fd19c4f9c6`  
		Last Modified: Wed, 11 Oct 2023 03:57:04 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9d706d8cea409c86409f061201a999c5fdfc900eeb9cd2c8d7c214bd462f3b`  
		Last Modified: Wed, 11 Oct 2023 03:57:04 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93fa899ae2056b59330f20c6e4a27ec6737929f17b7fa5a275baca12f8b1eb`  
		Last Modified: Wed, 11 Oct 2023 03:57:04 GMT  
		Size: 70.3 KB (70294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f049fc80168b8466bfbf3fd6b202ac8273bc9bd873e579290c2df3cb795a69b`  
		Last Modified: Wed, 11 Oct 2023 03:57:02 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d420eb4bc08ad8657d86af679a037777a0aabbc49c803e462db0bd08cc149`  
		Last Modified: Wed, 15 Nov 2023 03:48:58 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a105100ed34d614e5e5f3ee8dd12d20a80a8759c1acf3b1613b7bb58df6cd5`  
		Last Modified: Wed, 15 Nov 2023 03:49:26 GMT  
		Size: 200.0 MB (199989084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdec17c50a1c52ca60c48bee9e5f0aa2d1bef712dea53a9b7e1d429cacf14b03`  
		Last Modified: Wed, 15 Nov 2023 03:49:00 GMT  
		Size: 3.9 MB (3852140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b990e1f7a9d6604368b5836d91c3fd79803d964dbc6c6b8305d583c72142fc`  
		Last Modified: Wed, 15 Nov 2023 03:48:58 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
