## `eclipse-temurin:19-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:e09b884899753195c64094f2ed9c9ecc057552d40c4a9e7c381d6c8468604cae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:19-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:5c89315b0908551653d175485bac334c9228e7a15169ec03a15b73c1a07d07d8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167446828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18ad78a7f44323a0970b04f1349628f3e1da24b525d0f45d0a02a35c062a618`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:39:50 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:39:51 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 15 Feb 2023 23:39:53 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:40:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:40:05 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:41:21 GMT
COPY dir:904161e5243ae36448a284ab932eb54925cce61a8b841396759eee721890e3f8 in C:\openjdk-19 
# Wed, 15 Feb 2023 23:41:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab91262862cc0e1158f4869edf93e820c80fe8cc5360acef90052f4d26d837e5`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58929160bedb85968bc7fd10c682785c2a1ac5f89d9d2736265bcb99196a55cc`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea29e5d115afd492396980741a4cfb3b8d1d12df5c7887739565ac1234ea0f6`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83afce58205f8116dc64c080dd9ef9502447b4c292108bd5fba82c1e9b19f546`  
		Last Modified: Thu, 16 Feb 2023 07:23:44 GMT  
		Size: 83.7 KB (83726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d476cdc226464e55897a95ac3eda65bf7cac4ff190da662c7525c31b898b7`  
		Last Modified: Thu, 16 Feb 2023 07:23:43 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03c068852e144830b376b652a22d7168ddc1164f2763bb5949c2c9b7eb9ec16`  
		Last Modified: Thu, 16 Feb 2023 07:24:33 GMT  
		Size: 45.1 MB (45147655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dc1a9c46bc817767cb6af00eb9baef288a42de43f8c5ba5a22058ede9c6945`  
		Last Modified: Thu, 16 Feb 2023 07:24:21 GMT  
		Size: 90.5 KB (90539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
