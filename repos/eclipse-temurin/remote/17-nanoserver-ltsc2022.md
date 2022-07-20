## `eclipse-temurin:17-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:329795c8f37545edf884431027568d7707b9f44435b86fc4085568057e7b021b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:17-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:33d3572ba8860cb77a936819374a619661d2ba1245269dd2fe3bf8c0aee6258b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303403609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e24d4da157d93eeada458b503f6327dd2b69b609d30e69a5c46b9732deefbba`
-	Default Command: `["jshell"]`
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
# Wed, 13 Jul 2022 15:25:16 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 13 Jul 2022 15:25:32 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:25:33 GMT
CMD ["jshell"]
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
	-	`sha256:38b694fde26e11baf49a173c5e6e64f4f870fac5037fc3ec8e2d1b03afe0d28b`  
		Last Modified: Wed, 20 Jul 2022 12:56:15 GMT  
		Size: 185.2 MB (185203946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b620d2dedb32ac1b4bb378bdbc1c371e6a07baeac9dae99c61c3ccd95a37fa`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 62.6 KB (62604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9b8d20b337d5816473c1f75be612ac4e2a6513f3cfc0d4a9630a6fb6fb9d9`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
