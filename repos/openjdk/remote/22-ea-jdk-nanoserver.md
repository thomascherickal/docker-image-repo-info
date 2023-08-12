## `openjdk:22-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:8a44c42f78ecbc06f500738fbbfdf2c64a1a74b8c1605ccc76cf46f9fdaf2c41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `openjdk:22-ea-jdk-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull openjdk@sha256:c6ba7077c0452897c1e3ea34f359b5f7b42181405ab3021df11fc74c268883e8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307231416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf979ce67c9373ff2c7d8f26d95de20ec3cd29def58e75ec6a27dea64112906`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Wed, 09 Aug 2023 23:39:50 GMT
SHELL [cmd /s /c]
# Thu, 10 Aug 2023 02:42:08 GMT
ENV JAVA_HOME=C:\openjdk-22
# Thu, 10 Aug 2023 02:42:09 GMT
USER ContainerAdministrator
# Thu, 10 Aug 2023 02:42:19 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 10 Aug 2023 02:42:20 GMT
USER ContainerUser
# Sat, 12 Aug 2023 00:02:50 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:03:06 GMT
COPY dir:c691daaa319eaae4d4c3e5ae9ad607648e594c18de4183e3ed47fafba9a73453 in C:\openjdk-22 
# Sat, 12 Aug 2023 00:03:24 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 12 Aug 2023 00:03:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e08c5247c8c7d832882da17ac85015e9dd4d4dfc9e4114fc14746eb2abded`  
		Last Modified: Thu, 10 Aug 2023 00:21:01 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a07a6ee55409326d8105cc13d850b1705bbe4498575cf2e27bc34e78a1b5063`  
		Last Modified: Thu, 10 Aug 2023 02:50:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f896f4ed09b9390bcd098f89bb4624ae91e82cf7a9c4588ecdeeaa28378701`  
		Last Modified: Thu, 10 Aug 2023 02:50:15 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa6961892f2fba93ceeaf5806dc38793f041309ff787a61ccbd94e178ffd4af`  
		Last Modified: Thu, 10 Aug 2023 02:50:16 GMT  
		Size: 71.1 KB (71084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d01d10dd6ecb83bb10dfbaee0c9743aa78c0fb19d3da95691428a5cb7c9e078`  
		Last Modified: Thu, 10 Aug 2023 02:50:13 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196227f3999f1cc1f14383bd39fc302412a8b82bcd2bb23aa54f28681ae50143`  
		Last Modified: Sat, 12 Aug 2023 00:09:53 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6865b1830f247f3bbf0cb767406bf6f6e1f0011c0feb578049535142a9c70e`  
		Last Modified: Sat, 12 Aug 2023 00:10:15 GMT  
		Size: 198.8 MB (198848943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b81619c50ec6ea073894fc0759c7ce0316c32419fecbe8f62c5274757e903a8`  
		Last Modified: Sat, 12 Aug 2023 00:09:54 GMT  
		Size: 3.8 MB (3845054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c82469cda84aaf266bc459a857f029787065877e950e00136379eaa566cea6`  
		Last Modified: Sat, 12 Aug 2023 00:09:53 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
