## `openjdk:22-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5e530058304064d0f7d12a0562aaf307df6fc28283806645c700070a0b94ba6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-ea-jdk-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:25532809b39a8bc389bab8ef8f82ef936739b635c93bf5185830453f19e3b11c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.6 MB (307594570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c6b7a5fbd8b7f3972cf3a9422b4a524cf6a62b1adc604c318ab9bfe194e49d`
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
# Sat, 21 Oct 2023 00:18:20 GMT
ENV JAVA_VERSION=22-ea+20
# Sat, 21 Oct 2023 00:18:35 GMT
COPY dir:51c796d4e694629a270be125e9ab505cc45e5c0f1719efcf9b641397780da864 in C:\openjdk-22 
# Sat, 21 Oct 2023 00:18:51 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 21 Oct 2023 00:18:52 GMT
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
	-	`sha256:77b259172f223e90c6a2c1d2503e7cc13199d05881a7177ab618bfdac042d9e7`  
		Last Modified: Sat, 21 Oct 2023 00:20:57 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd8c22bfed98051489e3cc08172e2cf93afcd21c74164b1f25d9e2cd18a92d0`  
		Last Modified: Sat, 21 Oct 2023 00:21:16 GMT  
		Size: 199.2 MB (199212340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2541115f935285f403383df94cb48884f84e02864a62ba3889e7d465ba34ccdd`  
		Last Modified: Sat, 21 Oct 2023 00:20:58 GMT  
		Size: 3.8 MB (3840801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3975a616aea2d37416200468d32528e3f60a619f6c8514f145b04b1c175209dc`  
		Last Modified: Sat, 21 Oct 2023 00:20:57 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
