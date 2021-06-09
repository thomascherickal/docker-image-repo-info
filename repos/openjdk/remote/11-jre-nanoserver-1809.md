## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:3e53a622dc260f1edcf450fa3e0dfc848b9dc62018ea07a1165bcb445e5522b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:9902162cf5eeb8e9ed9bbf3a6b5218276f037546a68bdabe12241556d037788e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142271501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df434d1e52719fd33737c4952bd18acfde75a6fcda3fa1ba43ba7dd606994570`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 16:52:42 GMT
SHELL [cmd /s /c]
# Wed, 09 Jun 2021 17:07:03 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 09 Jun 2021 17:07:06 GMT
USER ContainerAdministrator
# Wed, 09 Jun 2021 17:07:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Jun 2021 17:07:23 GMT
USER ContainerUser
# Wed, 09 Jun 2021 17:07:25 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 09 Jun 2021 17:11:04 GMT
COPY dir:571c7e6185a2af7262c9cf23b4b5a526bbe98eb6de01d009d885b85f00e96dbe in C:\openjdk-11 
# Wed, 09 Jun 2021 17:11:21 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:acc28506464ab4d21eaffeb562876f3408463a46d298d12ded7ac0e3dd3c1bd6`  
		Last Modified: Wed, 09 Jun 2021 17:25:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad583918d22c41d05de15b1f7ffa677183966a3dedf225b26a5519a067f707f`  
		Last Modified: Wed, 09 Jun 2021 17:42:45 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8778df58d2cd15cfcf59ff364ebb4bb0ecb5570777a764b821c865c7cd0c3f`  
		Last Modified: Wed, 09 Jun 2021 17:42:45 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0f02558b6ba1a58df9715490f3372511b0d11cdc714717442cfa31eb6b57aa`  
		Last Modified: Wed, 09 Jun 2021 17:42:45 GMT  
		Size: 70.3 KB (70343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f889388780247f8a341983e88f1ddd4c636101289d9cc5aefc78e429f533ad`  
		Last Modified: Wed, 09 Jun 2021 17:42:42 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ebab4123d4948dc42976619fe7186a76bfc02683b7dd31bbf7838cb91c381b`  
		Last Modified: Wed, 09 Jun 2021 17:42:42 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25454acc302d8000b4806e340d37dacf7ae30fe8d2ccc63ac763f14f2ec9c0c7`  
		Last Modified: Wed, 09 Jun 2021 17:45:09 GMT  
		Size: 39.4 MB (39442073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a378dbddc6bd9a780e196eb209df4885345d6e5e4e4db648b06ce391d64acb9`  
		Last Modified: Wed, 09 Jun 2021 17:45:01 GMT  
		Size: 81.9 KB (81861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
