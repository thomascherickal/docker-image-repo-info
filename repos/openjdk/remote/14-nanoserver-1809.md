## `openjdk:14-nanoserver-1809`

```console
$ docker pull openjdk@sha256:b75688ef854946b5f044a58b05abbc1dcaf66f7df297ef0a26891d680e269503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:14-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:dc0361526b7f8777358afe580c83b38ef0814c9883e9ee76d1813f5ed816500d
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298476715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7987e214f0896e4ea349e0e9a35eaaf6058c85b54742466ebaadbc7417e90b2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jan 2020 23:56:11 GMT
SHELL [cmd /s /c]
# Wed, 15 Jan 2020 00:05:42 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 15 Jan 2020 00:05:43 GMT
USER ContainerAdministrator
# Wed, 15 Jan 2020 00:05:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jan 2020 00:05:57 GMT
USER ContainerUser
# Sat, 25 Jan 2020 04:11:58 GMT
ENV JAVA_VERSION=14-ea+33
# Sat, 25 Jan 2020 04:12:57 GMT
COPY dir:220cdcea4ce11598372496c4c00d0df869272a922d7dc4660fad5ebcba647353 in C:\openjdk-14 
# Sat, 25 Jan 2020 04:13:15 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Sat, 25 Jan 2020 04:13:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:764e25aa4e95684bd69a4d130dc1c729bfaef95293d9c76c4d2a12ced9e3a9ac`  
		Last Modified: Wed, 15 Jan 2020 01:51:06 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f3a5df9926db070e4016e42e49a7d9ce0131f528e644ae4388774831b6b46e`  
		Last Modified: Wed, 15 Jan 2020 01:58:21 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c21d67a14cad5558f706984eed7f97aaa2665e4b4cf1a7a1d21888c5e2c02a2`  
		Last Modified: Wed, 15 Jan 2020 01:58:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ffd38236cfc5913ab84e035b74a0bddf197bbfffdd8e9e8b151cc30bbf8adb`  
		Last Modified: Wed, 15 Jan 2020 01:58:20 GMT  
		Size: 66.5 KB (66486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8510d836b27dbac14cee7131c4209ebf2081c2ba957f75e05cbeff605e5320`  
		Last Modified: Wed, 15 Jan 2020 01:58:18 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07fc6ab813840c974b0d5311f3b9be5fd6d6af18e909afba8b6e1979cc4c40b`  
		Last Modified: Sat, 25 Jan 2020 04:23:55 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82b35712eef551ee4b0a1d5452233cb51b448d37155abde6cba7577e2e5bd31`  
		Last Modified: Sat, 25 Jan 2020 04:24:16 GMT  
		Size: 193.9 MB (193903790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc99c3c13e56f36523928661cf2a996a63d42992d1daea9c4491d94476fcb5b`  
		Last Modified: Sat, 25 Jan 2020 04:23:56 GMT  
		Size: 3.4 MB (3446554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acdae5cf5531b22ca0b77b9ed05c2b518fb1dafaecac869f4e084a4d3bc9665`  
		Last Modified: Sat, 25 Jan 2020 04:23:55 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
