## `openjdk:23-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:3d3a1c2c8cdb1fb1d86adcac46f9eaf1c6467cdefea102afb623c2e6b5fce4ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:23-jdk-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:0a72c4bcdbf4baddf117f71ccc96ab3070513974835ae979f0746edda9ab4121
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305849052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96848cf345ad2a78cbc5f677c43038cd041fc602167c22ae808734c73a9280d4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 02:13:28 GMT
ENV JAVA_HOME=C:\openjdk-23
# Wed, 13 Dec 2023 02:13:28 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 02:13:39 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Dec 2023 02:13:40 GMT
USER ContainerUser
# Wed, 13 Dec 2023 02:13:40 GMT
ENV JAVA_VERSION=23-ea+1
# Wed, 13 Dec 2023 02:13:55 GMT
COPY dir:c1af40c3dd3a5b960ebf976dd48a5f1482d7c7d93cf37ee2fe2c47c56a119861 in C:\openjdk-23 
# Wed, 13 Dec 2023 02:14:09 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 13 Dec 2023 02:14:10 GMT
CMD ["jshell"]
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
	-	`sha256:f0f61f582714c261ab3e53b770d1ca63d69c74265a2e4ec43efce45c9b2dac65`  
		Last Modified: Wed, 13 Dec 2023 02:22:33 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe7ce1578d9ec92511b00685dced5f90e537504618d931c93d2aa038ef647a8`  
		Last Modified: Wed, 13 Dec 2023 02:22:32 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73126db162f3a7a9ea882a984268769902d6820c051fdd7f66bcc2c3ad2041df`  
		Last Modified: Wed, 13 Dec 2023 02:22:32 GMT  
		Size: 70.3 KB (70312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11d7554cd7d412ee10e2776f5aa1ddd660d36b86541cee636786ffecac2f53e`  
		Last Modified: Wed, 13 Dec 2023 02:22:30 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15e15e121c790ad04228542527f80863a4376ef9c1e24849bc2e2b24c8ff43`  
		Last Modified: Wed, 13 Dec 2023 02:22:30 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912a2e60a9dd186297baf4c27ff433b07b706baec3b7ecb45ee3293e6b123279`  
		Last Modified: Wed, 13 Dec 2023 02:22:50 GMT  
		Size: 197.4 MB (197414928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30873b160f9d628780673d7af31fd7c091578be84f954b6fbc981b852f1e11d0`  
		Last Modified: Wed, 13 Dec 2023 02:22:31 GMT  
		Size: 3.8 MB (3846759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07424fc436bf1dcc25adcdb07b5ae67ca342a7e12c4abce2ed4c171ade765d`  
		Last Modified: Wed, 13 Dec 2023 02:22:30 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
