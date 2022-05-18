## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:573cecdcbdca7db537bf0f08a596ceb41a16b22f3f154159eddfae7db4504cb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:59ea79ac5aa81289a135946f75f4da3c0fc36f01486f1749e50685582bd29e8c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.9 MB (217937583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c31656a0b040625280f71a3e3a12569669264ff8f5389bd85347e19bfb9144`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:21:55 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 15:21:56 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 15:21:56 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:22:12 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:22:13 GMT
USER ContainerUser
# Wed, 11 May 2022 15:22:24 GMT
COPY dir:fe4a23cbc3aecb3ea1bcf0dca600117ebc14653b599151b614599054d6b82722 in C:\openjdk-8 
# Wed, 11 May 2022 15:22:42 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac36429f933755f4feb3856e62dcb854cd0c3ded07044ef3022b326c9be841`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf983a75185f46dcbd353c4168808c2c98c7bcc1379841008d4f84d61b0e2df`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e08e0e9837cbbdd01d54b4e3bbd7f199b280f70ac9ce2fecc568f676052612`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f802bf7ddce7178c0877e68417448396eea5e1058010f5a9c34b8410373a3d`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 99.6 KB (99580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8ac175dcdbc2fb1317b51dfac0b2b68e6a36afe2e8d00e44514e951e7d6c5`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7c235d552f696f3f0ffe2811c40450d11cc11f20f651ad74b8c970d9b8a57d`  
		Last Modified: Wed, 18 May 2022 13:44:12 GMT  
		Size: 100.1 MB (100076408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb38c9a2defa6685289a59184cfddbb822d007d1e63ee4d8532e9e5df084413`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 68.8 KB (68833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:810d2b70b43f5b4fc7e85e33ec0a9890fa66c3194ad71394e2c1339db29ca732
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203381576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d398dd0a261183066851d681511910d8d52c25ef97d1a0f630734619585e5129`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 14:49:50 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 14:49:55 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 14:49:56 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 14:50:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 14:50:08 GMT
USER ContainerUser
# Wed, 11 May 2022 14:50:19 GMT
COPY dir:fe4a23cbc3aecb3ea1bcf0dca600117ebc14653b599151b614599054d6b82722 in C:\openjdk-8 
# Wed, 11 May 2022 14:50:43 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8f2d99fa851deac0639d979721826197aba4963756d87edeaf12032faedd61`  
		Last Modified: Wed, 18 May 2022 12:48:04 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3f910a21f3d10321cc1617d1b47c075fa7cec8b190d21a0f8807a4af23b1a3`  
		Last Modified: Wed, 18 May 2022 12:48:04 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6196adacbbe2e54691328cdb81fa066ff43b86a6845d03f35d6ef4aeb75f39e4`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc662c0e9d3403199980e18b76f971e116138abeab04d82a9c20c3e10cf141f6`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 71.6 KB (71624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104a305619c88b65c3abb22985c69844c5289590d3d6657759e618aa0d59427`  
		Last Modified: Wed, 18 May 2022 12:48:01 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9dd42065f0f04a0fed48f01db6e73874dce61c6471bf2643b2eaa72456e36f`  
		Last Modified: Wed, 18 May 2022 12:49:52 GMT  
		Size: 100.1 MB (100078208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640d6635e3924f07bb36ad9f72a1adbda37cbf51321088e20668f180a4e6bcd2`  
		Last Modified: Wed, 18 May 2022 12:48:02 GMT  
		Size: 92.2 KB (92168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
