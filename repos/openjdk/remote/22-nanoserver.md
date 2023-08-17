## `openjdk:22-nanoserver`

```console
$ docker pull openjdk@sha256:8fb56ca9dc417b92a02ad5acde2e37260a8fbd1a396df9457d426361a86c2b68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `openjdk:22-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull openjdk@sha256:d7b2ce11e3c40969b9e5e91f0e4fc052fb83141d8852886085ac325d27875068
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.3 MB (307261894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6246ced69d4ef7a1da813c54df90db668672a4a1a774d38396d0eca7913dba13`
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
# Thu, 17 Aug 2023 22:26:33 GMT
ENV JAVA_VERSION=22-ea+11
# Thu, 17 Aug 2023 22:26:49 GMT
COPY dir:e45447278ee024c0de0163f1df6877113da8495a41e146166896cc0a33ba6f7a in C:\openjdk-22 
# Thu, 17 Aug 2023 22:27:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 17 Aug 2023 22:27:02 GMT
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
	-	`sha256:4e1a035b020dea700bf1340f772c64c106ac78e8de42db51165220230a2a1cc6`  
		Last Modified: Thu, 17 Aug 2023 22:29:41 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916bddef1977691bbb53c5a26e2479fb7b23f52b8dea72306019915496c88493`  
		Last Modified: Thu, 17 Aug 2023 22:30:02 GMT  
		Size: 198.9 MB (198890139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2582d16939ae017680a3c91924f151917c2637d09cd16b776113b9f3efc568d3`  
		Last Modified: Thu, 17 Aug 2023 22:29:42 GMT  
		Size: 3.8 MB (3834374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbf05effd8b7994df0bde279b64ab7c43a80d9a6a127819c82433311450a496`  
		Last Modified: Thu, 17 Aug 2023 22:29:41 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
