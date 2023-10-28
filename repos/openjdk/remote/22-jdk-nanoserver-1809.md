## `openjdk:22-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5a7d57c84c83efcae2a9b843a778b82ef5227ac02a845d8447867baa158fa0a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-jdk-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:e0fcdf9dbb64bbb18cf6a81416b6f5ac097fdba21702d3b121dcfd6dca7f3fe6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.8 MB (307845187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fadb2f8a07438b5baabefe7eaa52714292eeb34c628909ebc4f6088179252823`
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
# Sat, 28 Oct 2023 01:17:45 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 01:17:59 GMT
COPY dir:60cd34c312dd681322e594f12957905921041a928364f18b736151f02b5d75ca in C:\openjdk-22 
# Sat, 28 Oct 2023 01:18:11 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 28 Oct 2023 01:18:11 GMT
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
	-	`sha256:ca49a8c2a5d8dadb81c503fe8ff605aa74f94818458fb1431771783f269866f8`  
		Last Modified: Sat, 28 Oct 2023 01:20:10 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98ea1c937e90b90df0b6756a4b4ebb7fe046b458444464d1d827eb2e3e82458`  
		Last Modified: Sat, 28 Oct 2023 01:20:27 GMT  
		Size: 199.5 MB (199461376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee2a26d52e88d05e4ab1036c6fd48e224238de2ec661aff9cb7cf3da96a09b`  
		Last Modified: Sat, 28 Oct 2023 01:20:11 GMT  
		Size: 3.8 MB (3842445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bb7dcd9df3fd0da9eda087da09d14c08baf9a41f1120a77d32e260ad43abbe`  
		Last Modified: Sat, 28 Oct 2023 01:20:10 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
