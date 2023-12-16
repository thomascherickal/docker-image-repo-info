## `openjdk:22-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:6a9f842278b67842d6835aa751aec6dea75995958fb18b9d6f5b8c5e9bb89ec4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:22-ea-jdk-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:ce51e83cf9ca6f551eadac2efee313857be96625e17676bf6dbb32f3e20fb88d
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305812707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a587f79464747f0d823f49aa7a5e1e83f49908066234c664be4b167edfccedf`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Sat, 16 Dec 2023 00:02:19 GMT
SHELL [cmd /s /c]
# Sat, 16 Dec 2023 00:02:21 GMT
ENV JAVA_HOME=C:\openjdk-22
# Sat, 16 Dec 2023 00:02:22 GMT
USER ContainerAdministrator
# Sat, 16 Dec 2023 00:02:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 16 Dec 2023 00:02:25 GMT
USER ContainerUser
# Sat, 16 Dec 2023 00:02:26 GMT
ENV JAVA_VERSION=22-ea+27
# Sat, 16 Dec 2023 00:02:35 GMT
COPY dir:c3183e21daf82f91c89dad19d404dd9cded4db3b3e3e8aac85f37fb9729a4bd3 in C:\openjdk-22 
# Sat, 16 Dec 2023 00:02:40 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 16 Dec 2023 00:02:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16719ce012233e5c9ece457f4bdbe00ad26bac9b32c9afac49cc0b6df1c212e`  
		Last Modified: Sat, 16 Dec 2023 00:02:49 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6dd64405622ed120353496aafa8078b886d2be2b3e5568dd8bffbc51ccce85`  
		Last Modified: Sat, 16 Dec 2023 00:02:48 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f848275bc36ecee14bd713702c5c1bb61b7b124f4f85392108dabe6408597`  
		Last Modified: Sat, 16 Dec 2023 00:02:48 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108f36efba2131f2d6f482957cda55efda76b07b624514ea73d36a1e3e9e5bac`  
		Last Modified: Sat, 16 Dec 2023 00:02:48 GMT  
		Size: 74.2 KB (74167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe5418376f65e14643c0431c3242a67f0235d50ce21b1ce5ab5ac7bade5c944`  
		Last Modified: Sat, 16 Dec 2023 00:02:46 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c845f4bd0f6b4887ad7163f217519166a7517d952c184105090d9336b3ecb73`  
		Last Modified: Sat, 16 Dec 2023 00:02:46 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6aaedd2d372bcc15afa4f773f9dc359c76407a9912882b8c007bb52a0a9864`  
		Last Modified: Sat, 16 Dec 2023 00:02:58 GMT  
		Size: 197.3 MB (197325732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f050a9ea722b888c3afafa41274acd2b0e936a0e07367d17b1c80df49573e1`  
		Last Modified: Sat, 16 Dec 2023 00:02:47 GMT  
		Size: 3.9 MB (3896474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c17d7081599453105e144e0964f3e6ba41b869dac1174c0ba27c1a22715a0c8`  
		Last Modified: Sat, 16 Dec 2023 00:02:46 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
