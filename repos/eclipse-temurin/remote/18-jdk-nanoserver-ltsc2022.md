## `eclipse-temurin:18-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:f2bfb943d113ae8373c9efcca6481c7fda16399ce4f79c48a812edd45de06804
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:18-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:5577e9d84e1aa08336bc5f0121103fc66c3d4f56f1636003fde836d23da2a550
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304609256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c4b9283d2a2777846cebc1a237534f2dd13ff966d12adb25d1080bb94ede6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:26:12 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 13 Jul 2022 15:26:12 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 13 Jul 2022 15:26:13 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:26:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:26:26 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:26:40 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 13 Jul 2022 15:26:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:26:54 GMT
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
	-	`sha256:d4a37404d68858bede1ad1437473f24263342c9ab87d857a1d927012722b7d36`  
		Last Modified: Wed, 20 Jul 2022 12:56:49 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f17491f72356143169854ffe7321bb9181ddc40335ae4bcea24030d3d6b1840`  
		Last Modified: Wed, 20 Jul 2022 12:56:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac7753d08df63b45afd2c8942826ac22d39087db7317973879ca142e399596f`  
		Last Modified: Wed, 20 Jul 2022 12:56:49 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e0a75f48ebf388491c76565fa592c048058f32d9c048e06b79e06155b219bf`  
		Last Modified: Wed, 20 Jul 2022 12:56:46 GMT  
		Size: 78.3 KB (78326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fe3a8a776aafd8edfdee821e8c2fbfbcac4d4bc678b88d52fede2d400e7b4d`  
		Last Modified: Wed, 20 Jul 2022 12:56:46 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9ecea44392025f3f3bfd39d4dad10aeac9d5457e081cc2360074769bebc195`  
		Last Modified: Wed, 20 Jul 2022 12:57:08 GMT  
		Size: 186.4 MB (186416983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9e3490672bf58b7077f6ac615e2e5274c811be3ac4b8a4488bddcde17ffc1b`  
		Last Modified: Wed, 20 Jul 2022 12:56:47 GMT  
		Size: 60.9 KB (60940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee89aab8d47cc8fdb4e429ea8fd550dccd2f0440611d91367391c30921b339`  
		Last Modified: Wed, 20 Jul 2022 12:56:46 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
