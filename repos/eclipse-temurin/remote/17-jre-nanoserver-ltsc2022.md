## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:95d81ca305c7eae9f60f45ebddf1c99f38fe2bf8afbe5ca46cc201e1bbba3536
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:ab9904aae9cb20c11ff4580ae31aa03fd56c5896d76d91259cd26d66e0e73b44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161322782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfcf4b51def0bab61392211c7b3a405d03096026743c534d4149a55ed095cde4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:24:51 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 13 Jul 2022 15:24:52 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Jul 2022 15:24:52 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:25:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:25:03 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:25:50 GMT
COPY dir:c21630f3252a44226ea19120d87b000e49aedb9d546bbac0f6424fd80f37c64d in C:\openjdk-17 
# Wed, 13 Jul 2022 15:26:05 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:569505cbc9e1bcad1fbbdd7edca170e5a914864bcad2f53e1fc5d5816ecc8aa5`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd304d30701ca0c21239a9af97bd54b9d78f03979db6ff656d7e63f9cd0bd7e2`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69b032ede38561ad345ad0f5cc9ec55cbb7c381193c115d09c752d8718f399b`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e91de4a68cd7b1fd79bbcfae2f4f57983f5bc22f8b9442034e8ea2fc08e4`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6eac017f94e9ccdf56550efc861d11f10c2027f412c844a8a258249c5f541e`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 84.0 KB (83993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde92d157ca9d16443eea1808f120b1fd10463ad6480c26b750edbd8e640af9`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61392dc67ac6623ea1cc4c93c5a2c920877a5fa47db01d8616d02499dcc7dcae`  
		Last Modified: Wed, 20 Jul 2022 12:56:37 GMT  
		Size: 43.1 MB (43124924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f0a21842d88f05d365f0068fba26f407ad0de43a2507e37d6bb93b76479e3a`  
		Last Modified: Wed, 20 Jul 2022 12:56:27 GMT  
		Size: 62.0 KB (61966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
