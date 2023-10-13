## `openjdk:22-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c816188ee4de6f644da951fecd69d298532165fa084562bfdefd683804e50ff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-ea-jdk-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:8ab5a989e5b07252ea79a2cdf52837e4230ff1fb74f495157c879f5ded3ff831
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.5 MB (307532164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235d3ac477a7ab71d58f4f78073c7ee5e15bc35f2327fcd80c71e38328dfc5c0`
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
# Fri, 13 Oct 2023 00:36:16 GMT
ENV JAVA_VERSION=22-ea+19
# Fri, 13 Oct 2023 00:36:30 GMT
COPY dir:e05c7513b8e8266ed04bcda08bf7d39e28bc98f1737194a96bd8f74963061477 in C:\openjdk-22 
# Fri, 13 Oct 2023 00:36:42 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 13 Oct 2023 00:36:43 GMT
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
	-	`sha256:0ba41a9b08bca92c3c58bf0db4d5c7248bc6555b3bd322289826a093a9a888bb`  
		Last Modified: Fri, 13 Oct 2023 00:38:42 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e226ec8aa547d489ab1f55c683cba864ca2bada5630680b77d44adcbd5c14`  
		Last Modified: Fri, 13 Oct 2023 00:39:00 GMT  
		Size: 199.1 MB (199149991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5a7b63868b0e0c9573525f503372247287990a01683dda43dc2c050b4eef43`  
		Last Modified: Fri, 13 Oct 2023 00:38:44 GMT  
		Size: 3.8 MB (3840748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87e25cd96adab5a3258454f6b605f2930527093357bd5649f2baa869da685e1`  
		Last Modified: Fri, 13 Oct 2023 00:38:43 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
