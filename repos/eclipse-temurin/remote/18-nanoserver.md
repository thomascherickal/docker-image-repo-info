## `eclipse-temurin:18-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:e5686afbdfc4abae3d982cfb41ab8a90fe6aa7cc675c4694dd875eed99ebd6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:18-nanoserver` - windows version 10.0.20348.825; amd64

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

### `eclipse-temurin:18-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:4f74a347b0a873243713d9566f72f258396b5ca25f53f5b3abdd83341d5603af
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.2 MB (293215145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a367fefd6c9364bb0609604d588c6ec4df72e7d71168375ef79b787b28a901c0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:17:32 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 13 Jul 2022 15:17:33 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 13 Jul 2022 15:17:33 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:17:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:17:44 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:17:57 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 13 Jul 2022 15:18:11 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:18:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81ada5c064096d451a5fa939bb2790837e82189f9ccd1c0453eb5154fc7c61c`  
		Last Modified: Wed, 20 Jul 2022 12:52:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60535efa2c7f3be903ac8a6225348ea675f749ec497715f00a1402cca687cde`  
		Last Modified: Wed, 20 Jul 2022 12:52:33 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3256c5f48a4f1674ddd645c233cf689a35eb1cb2575801f0bb6ae53e72926cc9`  
		Last Modified: Wed, 20 Jul 2022 12:52:33 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bd69f3df6300a8b750eb2dce6451b8f1fa1ef0f86018b086d1570cbca255b`  
		Last Modified: Wed, 20 Jul 2022 12:52:31 GMT  
		Size: 71.1 KB (71101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c29e9bad6fff66a0ec3c325033dac234a0e6ba69ba10a83fa35d9e6a796a6ea`  
		Last Modified: Wed, 20 Jul 2022 12:52:30 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f8b190f545284bc3c5583412de21b08887223ce865c7457e924af5a7bf4c16`  
		Last Modified: Wed, 20 Jul 2022 12:52:53 GMT  
		Size: 186.4 MB (186423725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa0e996f3f351ba1a112a1bfc94c6955a502f4e91aa5227537fbf3e99cc75bb`  
		Last Modified: Wed, 20 Jul 2022 12:52:31 GMT  
		Size: 3.6 MB (3558438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d68424a601b6b0949b983122194534574a9efd0fc0602325dbd70b465ef5dd2`  
		Last Modified: Wed, 20 Jul 2022 12:52:30 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
