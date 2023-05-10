## `eclipse-temurin:20-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:e1b160f3d8cd5bbd9d5f60c70aef4f1b09c9afe24a147fc7970bf9b10bea95ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `eclipse-temurin:20-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:b9ee0b6d8bb85b6dfcc1962e9d06cd728610ab40eedb3faa30bb51f1640cd966
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.4 MB (315432775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176226a4dc8658444e180a2d3de155cb93bf0613cff18f080060447fb2a7418b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 12:52:54 GMT
RUN Apply image 10.0.20348.1726
# Wed, 10 May 2023 01:13:54 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 01:17:33 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:17:34 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 May 2023 01:17:34 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 01:17:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 01:17:44 GMT
USER ContainerUser
# Wed, 10 May 2023 01:17:59 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 10 May 2023 01:18:13 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 May 2023 01:18:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7d382efe6974b94c05000b6a95c1fd28e1b8bb3e81cc4592b2aa1cc46b90192c`  
		Last Modified: Wed, 10 May 2023 01:48:23 GMT  
		Size: 120.0 MB (120001338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cfc306feea2a215b4a83a66480231042a4bdc8001d07d634086f52f1f5ab3c`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102b5285ff20b5da43698a254b019623d13fa0fff343e58f02364a7fade0f9a9`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed92b05a447b82514f3ed09c8800f00450d6dfaf4a834d5c4e89a7721c06362`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263c8320754a70ba87c2bfe5f942d9c40c5ba1ee480bbae87511d66fe8e18bbd`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78515dd5692679ff78e48ff2ec16e74323946877ef490c6f5deaa177d7617ac`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 87.3 KB (87340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789563d9e96a6480dbdb98188690acdd4debcf1e4f88704749b2dca25f108111`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7270b423dab2f7e86cbe277fdbcf9ad93d1e727a5aa5540959d5b6e2aa358952`  
		Last Modified: Wed, 10 May 2023 07:06:31 GMT  
		Size: 195.3 MB (195277033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b160eda48493090f780728650a9270b3ac3c39d790c40c43f079420d136b06`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 60.8 KB (60792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9c7e79d50c3443432bbb6fc12f02d2e09e97d0a37aeabfb38104791d27533`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
