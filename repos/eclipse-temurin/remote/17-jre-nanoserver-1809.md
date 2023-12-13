## `eclipse-temurin:17-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:d76af6af5898da29f3da494fef133c65508f6b9d4d747bfb461dd43d35acb9aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:17-jre-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:5f81d860b14cd04ec1aa8984e5221214b307efb38fdb75de302f036bcfc74f95
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150957587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739568b7c3f20f88718a854129db39897a68a13d730994253ec215a653d0b090`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:33:45 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Wed, 13 Dec 2023 00:33:45 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Dec 2023 00:33:46 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:33:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:33:55 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:38:33 GMT
COPY dir:d3f692ac99669197443250e31cbc5c2f5282787fd78589cc9b6c2e91236738f4 in C:\openjdk-17 
# Wed, 13 Dec 2023 00:38:44 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759cb4ed6491f9e54a454d0a71a8f970fc9d89d448f7d1da03704676a4513976`  
		Last Modified: Wed, 13 Dec 2023 06:40:07 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e12f88eba068765157a3c2a27bb0ca228689ff4250045d91de871928ea48ea`  
		Last Modified: Wed, 13 Dec 2023 06:40:06 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428c08e8f690f917aa2abf284c604a53bf62395b8736ae4c634aba98fb676dfa`  
		Last Modified: Wed, 13 Dec 2023 06:40:06 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bd2de65c197e07a96b40407e68be5fe33e9941f893e7904f8b7ddf02f55ef8`  
		Last Modified: Wed, 13 Dec 2023 06:40:04 GMT  
		Size: 68.8 KB (68793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d11b5633cc89d40e3aefdfcc7358f6d8245c3991460c275d523dad5f445bde`  
		Last Modified: Wed, 13 Dec 2023 06:40:04 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3c5d24d06b43f4e0bc18037c08baccfb8d79d62234ac9ff71a63852ff8b86`  
		Last Modified: Wed, 13 Dec 2023 06:41:20 GMT  
		Size: 43.4 MB (43396757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb74c0820c7d89ade0261620ba158bb3988dc3e3cd263acad6580ae09f9ed2`  
		Last Modified: Wed, 13 Dec 2023 06:41:13 GMT  
		Size: 3.0 MB (2976680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
