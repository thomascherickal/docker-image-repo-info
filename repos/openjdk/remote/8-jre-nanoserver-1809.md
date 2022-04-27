## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2ffd2828218c7a1678ad2ba4924b393ed813cf6cb0b5c4094bf10d2811de7402
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:9159d452a1650284424576603ff88bfc521213c914f6e6a6d50c440fe5c20a87
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141526704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:521d41de0a4d8185ddbfe24192e9fe2e2d4c5aa3cc4398f02159e340e08a307f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:21:37 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Apr 2022 17:21:37 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:21:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:21:44 GMT
USER ContainerUser
# Wed, 27 Apr 2022 22:19:38 GMT
ENV JAVA_VERSION=8u332
# Wed, 27 Apr 2022 22:22:32 GMT
COPY dir:a69662fb25cadf36484d90c7c9990719015f86fa8a02dabf235af3b8f20f255b in C:\openjdk-8 
# Wed, 27 Apr 2022 22:22:42 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65fb95ee42514e5278fb1f68d4225d0a5bba71921defb635d841ca30789226f`  
		Last Modified: Tue, 19 Apr 2022 01:19:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b00dbd36f2154a4eabea44e9a5d88c98927e03b469bb16de373838d0f29d1e`  
		Last Modified: Tue, 19 Apr 2022 01:19:34 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c635236ace6c57e8af5a6a467722bb1484d5ae5aaf133d60a5475aef5f4d2c4`  
		Last Modified: Tue, 19 Apr 2022 01:19:32 GMT  
		Size: 72.2 KB (72156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9131ef298cbc9163210fbeb93d70aed6922673cebc88b8563ea8ea489357b1c`  
		Last Modified: Tue, 19 Apr 2022 01:19:32 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916d4a5c260a30f1a16a40718d959ff928c900be9607f848103cd78e06b236`  
		Last Modified: Wed, 27 Apr 2022 22:28:39 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae83039fc80705923da95c7891b0ee553922b16d02722d59cd0656f8e244bdc`  
		Last Modified: Wed, 27 Apr 2022 22:32:29 GMT  
		Size: 38.3 MB (38293954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cc1c4343bfa5c7374f09ad7c57144c5962afdb02b5abd74754777bacebbf39`  
		Last Modified: Wed, 27 Apr 2022 22:31:47 GMT  
		Size: 58.8 KB (58799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
