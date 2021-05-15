## `openjdk:17-ea-22-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:78c0ba6c4743d51d81f8df0c35fd3fcedae3f09bdae3b43b842c6ab9dd4152d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:17-ea-22-jdk-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:85268e7df6861061ed97a851740b138ed0e14e63812c4e2e3f27f4cb28f3c3f7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286115237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d26eea2183be0f4f82f3eca7200e89df954c2848b90a42aa0ec7ed8709776e0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 16:42:56 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:42:57 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 16:43:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 16:43:21 GMT
USER ContainerUser
# Fri, 14 May 2021 19:20:22 GMT
ENV JAVA_VERSION=17-ea+22
# Fri, 14 May 2021 19:20:41 GMT
COPY dir:72dfce67199c242dfb6158fa7a1125ede397ee804bf77b8c60478afb596e1894 in C:\openjdk-17 
# Fri, 14 May 2021 19:21:19 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 14 May 2021 19:21:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea91a7775c05d55a850a2983043468ce6ded7406743836cf8f33afb037aba1a8`  
		Last Modified: Wed, 12 May 2021 17:16:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0a5b4dd190af3527c02bb783babc5d88014a4de37555355c2f7a59dd21449`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab5fc14de7c93823ea1579b64e1e79017e9738a39e5d165aeed23c15bf7ffd`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954cb2ae96dfb0f537ce02738b91077c41cda7743ff097b99d8a6cfc74e211f`  
		Last Modified: Wed, 12 May 2021 17:16:40 GMT  
		Size: 69.5 KB (69533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95581d66523cc5b44afdfbd1f1e7732689ad5d73bf1c1352ef8f1e669dceede2`  
		Last Modified: Wed, 12 May 2021 17:16:37 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea00399480b426067523c0f58d4b5a20cdd1b299765838b2976427c5be055893`  
		Last Modified: Fri, 14 May 2021 19:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2a3278d18533f6f32f0d7ec0035285189028d0a15bdc8121236f006b57285`  
		Last Modified: Fri, 14 May 2021 19:32:43 GMT  
		Size: 181.0 MB (181013161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba0ed79aed49277db3456100cfa2ae8a54706a6c2a1fde37adbf1457d968bf`  
		Last Modified: Fri, 14 May 2021 19:32:24 GMT  
		Size: 3.7 MB (3650409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b154e8c58f659a31e0f98a4c0d13c55ca00a99dead3a9751cdb2b84757a161f`  
		Last Modified: Fri, 14 May 2021 19:32:23 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
