## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:9a59be8fde300681bf9d6068ba72378bdd4ebc5d1ae37e23415dbadda0400f19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:cc4827c7f25a0e602bd9237786a0d445c142e58a46626e2a57e338caf1a1d974
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310418476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9058af95a8c79f1e64327b44412fa88514824c86a740f1ae40d3ddfb4fae5933`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:23:21 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 13 Jul 2022 15:23:22 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Jul 2022 15:23:23 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:23:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:23:34 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:23:48 GMT
COPY dir:1583ce76f01a2d0a0742f7b70646c210ef8c619565a381c37e5a1156f6ec4636 in C:\openjdk-11 
# Wed, 13 Jul 2022 15:24:13 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:24:13 GMT
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
	-	`sha256:e2f1d7ed18ddc442fb4f4a640cfebca04ef586c37324c6ac27e1fc63300f3d45`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8277017e15cde483b8b44a6115b95f99675f7005ee4b62a4a81bdf97c1eac7dd`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f99951dad87e30f27404d1dff1852f7351149213eaf5499bc67a89fdfcf21f4`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7b5079facd10880a84cf3d272bad70b33a62fc144d3fc961f2f551d6357c7`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 77.7 KB (77660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd41caaf3f7ae470605597ef2dea693acef178db876628d3f379f7a4e9a70711`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c0e981f98ca670b7d2314d3f910b8f6f3896638a21968f4e4d0b7317289de7`  
		Last Modified: Wed, 20 Jul 2022 12:55:21 GMT  
		Size: 192.2 MB (192225424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4aeaab39ce92bef20446e231540ad0072ff0074922e0370f4992311732fb41`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 62.4 KB (62417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76179379fbc7e35539371ffa8c000f93b1df1e0c3e22115fe63c38403fedc13`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
