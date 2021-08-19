## `openjdk:18-nanoserver`

```console
$ docker pull openjdk@sha256:e13cde8175c9149746c4c5c4d05297f27376540f7cc1bcdd0aee78322d39dcb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:18-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:7c4f4d1c6f7f69466621349417079148f16f5107d6e59d2bb7e01451cab7738d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289054973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026ac9b043dff9af47702906f2956c6fb3165c688094aaa2977a5f03bee77b88`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 17:30:38 GMT
SHELL [cmd /s /c]
# Wed, 11 Aug 2021 17:30:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 Aug 2021 17:30:43 GMT
USER ContainerAdministrator
# Wed, 11 Aug 2021 17:31:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 Aug 2021 17:31:09 GMT
USER ContainerUser
# Thu, 19 Aug 2021 21:20:19 GMT
ENV JAVA_VERSION=18-ea+11
# Thu, 19 Aug 2021 21:20:40 GMT
COPY dir:ca4e1784e2eabb7051d38d88537ff2f3e428c6a89243a40ca74a81ac1c13ccee in C:\openjdk-18 
# Thu, 19 Aug 2021 21:21:00 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 19 Aug 2021 21:21:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae0a5a946be2ad0e39a8260e454c0060a31a9f7e5be75d1f9038dc13730abc0a`  
		Last Modified: Wed, 11 Aug 2021 18:21:28 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3e3ce6f906341a31b594d25772e87453477f92df500f7e55c033ee65d1f7b8`  
		Last Modified: Wed, 11 Aug 2021 18:21:27 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4140a377a80813839c51929577daa32b3f49ead3975b3b71a2106af7999f7c`  
		Last Modified: Wed, 11 Aug 2021 18:21:28 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeec1a666d3ea4495353e16515d8a87648b15d6c51c137b53bfba178aa5a36b`  
		Last Modified: Wed, 11 Aug 2021 18:21:27 GMT  
		Size: 68.6 KB (68571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bce606c6fc4ebc45e038cdeefb933ddc75feed60a9793ef5682fcacbeb615c`  
		Last Modified: Wed, 11 Aug 2021 18:21:24 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9bc17512bdc1ab5afa0d858c45601d3c317a1990b58d35259ced9f4180b1f5`  
		Last Modified: Thu, 19 Aug 2021 21:29:46 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef905d5317d23d5cf740ec36d37c9376f30d7772c09a0e906096103703d2f8ca`  
		Last Modified: Thu, 19 Aug 2021 21:33:08 GMT  
		Size: 182.6 MB (182623569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffed2c2a4b2d87a811774d2c36365646ad7bc8138f44ceb52f9c3ca9e745a68`  
		Last Modified: Thu, 19 Aug 2021 21:29:47 GMT  
		Size: 3.6 MB (3614939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cf65886ac7c21f234cf47c7b9ecb8114f7b635a9c05d5827abc4cd0f6cac17`  
		Last Modified: Thu, 19 Aug 2021 21:29:45 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
