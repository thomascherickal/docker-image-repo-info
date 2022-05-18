## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:74b1c9a82970172cdd8ff1c3f3ee9cce7d568a58f714cf8caa113ee180a324cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.707; amd64

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
