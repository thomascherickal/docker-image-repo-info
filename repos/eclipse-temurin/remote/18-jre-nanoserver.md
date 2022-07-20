## `eclipse-temurin:18-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:02b71bbcfd6c94264fa8d30d32ab499f2365a965ba7bb5b354ea194ff0c5a510
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:af5c5584f22ec4af663dd34e4a3167298f77adeb96c362018061f62550380311
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161230147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8908a7f2da52f0d0dc5c6f91d22bad4d135b68d7343a713478383d6ce7cfd343`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Jul 2022 15:27:10 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 13 Jul 2022 15:27:26 GMT
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
	-	`sha256:22fdc33dac26f8d4b893a3edcb5f3756a1126a7d0d3ecccb6acf8af6c034af76`  
		Last Modified: Wed, 20 Jul 2022 12:57:30 GMT  
		Size: 43.0 MB (43039203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42328b16b9ce5d7ae756906a7f15d6a4e7a75ee4dc9299c729f9ff6a5654f10`  
		Last Modified: Wed, 20 Jul 2022 12:57:21 GMT  
		Size: 60.8 KB (60788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:c5c23ec304748466d4b85fe07047dd375761d7e075c52e1fd01ea6f0caaa0faa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149214283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf4da5166c2e7b4b03fd3d0f7083d240f06d0436778d1b6ebe4ca1dd5c45d64`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Jul 2022 15:21:44 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 13 Jul 2022 15:21:59 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:6a07629775e0ef3574424b074ab988a03ac02d0bf678fbca89f9cc8cceffd4e4`  
		Last Modified: Wed, 20 Jul 2022 12:54:00 GMT  
		Size: 43.0 MB (43041251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee2ac13f34af4cda6e45cb055db378d82a056bc5bf4f3e30127bc7f25d8ed18`  
		Last Modified: Wed, 20 Jul 2022 12:53:52 GMT  
		Size: 2.9 MB (2941178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
