## `openjdk:18-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:7cee071603bf51262d2fa4729150e3f2e33dd848d4ae0f051bfc2cbc7ffdb9cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:18-ea-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:e150d4a69983584220c2536899cd08dd91ef0e3678f62223aeb712cccd707d87
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.0 MB (289036326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1ca5cf0805e5e43807bc6d321c068f502b702677b98236eb4917d5b8afccc0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 17:06:45 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 25 Aug 2021 17:06:46 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 17:06:55 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 25 Aug 2021 17:06:55 GMT
USER ContainerUser
# Wed, 25 Aug 2021 17:06:56 GMT
ENV JAVA_VERSION=18-ea+11
# Wed, 25 Aug 2021 17:07:12 GMT
COPY dir:ca4e1784e2eabb7051d38d88537ff2f3e428c6a89243a40ca74a81ac1c13ccee in C:\openjdk-18 
# Wed, 25 Aug 2021 17:07:25 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 25 Aug 2021 17:07:26 GMT
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
	-	`sha256:529f54617b19374dc6ae56b7cbadea820f6613c38ef8eb5b3780625f824e7f70`  
		Last Modified: Thu, 26 Aug 2021 00:39:57 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17928612bd587dae3533403ae499232eb58f410a5e0875cca4930241ef47caa3`  
		Last Modified: Thu, 26 Aug 2021 00:39:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b2868a6eab69d3ff3c1ab6e50f537ef7b5671cd3a888b7fa6fcc521e63759`  
		Last Modified: Thu, 26 Aug 2021 00:39:56 GMT  
		Size: 71.1 KB (71120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f7631bcd8fcfd1b84d19c43b45e42f54be2bafdb008157e4d2e8d7a64430a`  
		Last Modified: Thu, 26 Aug 2021 00:39:53 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ab9332009b43daf5ec998b7c6239668feec20c270fda42d4fa029897b8093a`  
		Last Modified: Thu, 26 Aug 2021 00:39:54 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea649884c60af09f5526aba0481827f8544d055a4903c86e727006e1f7d3b7b`  
		Last Modified: Thu, 26 Aug 2021 00:40:13 GMT  
		Size: 182.6 MB (182597489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c6d60e4b26545204292ec51b01858ab023a012f20d5cc3fc1fd425d01aeda5`  
		Last Modified: Thu, 26 Aug 2021 00:39:57 GMT  
		Size: 3.6 MB (3619718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a764c17d2469336c2659f46f6c360d0a6af317fed4dbc76b3ebff26d0e6efc4d`  
		Last Modified: Thu, 26 Aug 2021 00:39:55 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
