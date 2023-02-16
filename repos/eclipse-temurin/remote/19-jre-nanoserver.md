## `eclipse-temurin:19-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:f1171e8da8d7642a21abbcedad4ffe9eccd0f2655ae20392f16a88444053e700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:19-jre-nanoserver` - windows version 10.0.20348.1547; amd64

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

### `eclipse-temurin:19-jre-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:98db9f434286f107f41b6f3d705506d41c461d22acc649dda346cc92d67da498
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (154979812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fc5133f1050e6b643d69691fb9e56ff82e8272d6eab4df7d5959913b9bfeff`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:27:19 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:27:20 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 15 Feb 2023 23:27:21 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:27:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:27:33 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:33:31 GMT
COPY dir:904161e5243ae36448a284ab932eb54925cce61a8b841396759eee721890e3f8 in C:\openjdk-19 
# Wed, 15 Feb 2023 23:33:52 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fde067c8eccc1328d0a3feac3c80f546000512f6ef0b1530025028009882220`  
		Last Modified: Thu, 16 Feb 2023 07:19:18 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336cbf9f7dea0d8f28865cf51e08f21f5b6f61982edb0dccb7c0a4864cb7a727`  
		Last Modified: Thu, 16 Feb 2023 07:19:18 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4589e9856fbb0f5bcdf26dd4520c482976af27eeb93e52f20d90884e337afaa`  
		Last Modified: Thu, 16 Feb 2023 07:19:18 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0de03d87d6bdd47463da17f631588d1ce4a261db568810f4417ce88c060f706`  
		Last Modified: Thu, 16 Feb 2023 07:19:15 GMT  
		Size: 69.8 KB (69820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1ac02b962962f92732ced99f4eaaacac38765ded72cc31c7c7ce3e4b413308`  
		Last Modified: Thu, 16 Feb 2023 07:19:15 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7216ecaebf427c7cd287454b59863bec2d892c4553f4b285ef4cda7831bd1`  
		Last Modified: Thu, 16 Feb 2023 07:20:54 GMT  
		Size: 45.1 MB (45143456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398b93943d82033ec45158ae3c638edd276a16d9ae4cc9399c50ce2baa27a9a5`  
		Last Modified: Thu, 16 Feb 2023 07:20:44 GMT  
		Size: 3.1 MB (3086208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
