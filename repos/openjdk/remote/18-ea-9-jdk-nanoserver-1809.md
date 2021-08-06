## `openjdk:18-ea-9-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:1a7d5822659057f7e69a4cd9d5485df527a143b6fce4e6c306b8677cc1b7dd6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `openjdk:18-ea-9-jdk-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:277fa0228f03b98a19350e8d37d98f7fae79903553561c851e134da8c821b790
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.1 MB (289067560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b3f9bcbd19484e1b38092b0d5e03f2919e8240ec85da5ceddb9e6ff4535bb`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:53:30 GMT
SHELL [cmd /s /c]
# Wed, 14 Jul 2021 02:53:36 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 14 Jul 2021 02:53:44 GMT
USER ContainerAdministrator
# Wed, 14 Jul 2021 02:54:04 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jul 2021 02:54:08 GMT
USER ContainerUser
# Fri, 06 Aug 2021 18:18:59 GMT
ENV JAVA_VERSION=18-ea+9
# Fri, 06 Aug 2021 18:19:16 GMT
COPY dir:90ec8134647146eac9e668dce7afdccf7a2a64d110862971c025e25f054d7a45 in C:\openjdk-18 
# Fri, 06 Aug 2021 18:19:44 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 06 Aug 2021 18:19:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d8754fb12dd351c91bed29d92c703cddb135a78d8f056b6a3bf13a251c1d2d`  
		Last Modified: Wed, 14 Jul 2021 03:42:27 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89509de1f10eea36c6e14a8f32bc735a7e52e07235bb588c9dff480855c851c0`  
		Last Modified: Wed, 14 Jul 2021 03:42:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a172401c9271ad5ee8356c8f36a409f68259854e9de596e04069a2a176db3c6`  
		Last Modified: Wed, 14 Jul 2021 03:42:25 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247de649752bd08242527a227d09c6398c2676025c2527f3b65c5c8cd032886`  
		Last Modified: Wed, 14 Jul 2021 03:42:24 GMT  
		Size: 69.9 KB (69948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1baf3b57ea2d376291b5174f1db66c9b8d971170b6ec871bdbd1fc496e82d65`  
		Last Modified: Wed, 14 Jul 2021 03:42:22 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e3b929394f939744e5682f8516ade5fb32b2f2e4588d54d715b33df93598b`  
		Last Modified: Fri, 06 Aug 2021 19:26:40 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5a9e794a8571acbfb7e529cd3b919c4030b18865adec63fe27f7677decb3ea`  
		Last Modified: Fri, 06 Aug 2021 19:30:03 GMT  
		Size: 182.7 MB (182659409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd9190f98ba3350bad3053dc74ac141e5de2230f97751d57985718873750587`  
		Last Modified: Fri, 06 Aug 2021 19:26:45 GMT  
		Size: 3.6 MB (3605601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1e9009ed318829c6c2cce3e3fd0155fb1d67e1b9a97e2224476889dbdbf84e`  
		Last Modified: Fri, 06 Aug 2021 19:26:40 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
