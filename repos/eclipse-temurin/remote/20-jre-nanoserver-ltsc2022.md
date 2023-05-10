## `eclipse-temurin:20-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:ed847894b25cf294b92f289d6b8b5f985ec35f93758c685fbd304dc539302708
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `eclipse-temurin:20-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:1d88b431209517ea3c29f14e4f38f942ac4392d7629efafef44b30f0bafd9870
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165912611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ca197050a755bf925d78ee4bf7b42bfabc3593489e656d7a50344e81ab7223a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 10 May 2023 01:18:32 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Wed, 10 May 2023 01:18:44 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:d7ee82220916950af7b731231a181e6e39b764cc34c5d832b08ddb70890c2ad7`  
		Last Modified: Wed, 10 May 2023 07:06:50 GMT  
		Size: 45.8 MB (45764985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5965a51804686e8bfaeeb2619da75fe92c8a1675724a9a9146a60cbcaa946`  
		Last Modified: Wed, 10 May 2023 07:06:42 GMT  
		Size: 53.7 KB (53707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
