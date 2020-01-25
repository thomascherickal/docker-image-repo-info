## `openjdk:15-ea-7-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:6b6f934f03d7a9be87fb83acde3b2b8be5be433985893827687a746a0d4f9d32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:15-ea-7-jdk-nanoserver` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:a0a8822f8edeea3581de8702a069a12d05c6a96f30a22ff9e39a0631448d77fe
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298578138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f2e6b27c22762cdf200bed7f61aceaeca65ae21bd187d8d3e70eb2f7a99f43`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jan 2020 23:56:11 GMT
SHELL [cmd /s /c]
# Tue, 14 Jan 2020 23:56:12 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Jan 2020 23:56:13 GMT
USER ContainerAdministrator
# Tue, 14 Jan 2020 23:56:30 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 14 Jan 2020 23:56:31 GMT
USER ContainerUser
# Sat, 25 Jan 2020 04:05:02 GMT
ENV JAVA_VERSION=15-ea+7
# Sat, 25 Jan 2020 04:06:04 GMT
COPY dir:5b574b617c555195e82057c07cd207de30d13f1f806d05ca86d438ac74ff51f7 in C:\openjdk-15 
# Sat, 25 Jan 2020 04:06:26 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Sat, 25 Jan 2020 04:06:27 GMT
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
	-	`sha256:4f193e511d66e393e8623d9efd86f48f82cc15ceb19ee3a6ac9da7343da044ad`  
		Last Modified: Wed, 15 Jan 2020 01:51:04 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fab357b0406f3be040eca20b497e3bdd7e731b95865fbfbe83acf826248583`  
		Last Modified: Wed, 15 Jan 2020 01:51:03 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fed5c1fef1ff77da19cbdb310981f89c791b7c4206a8b99d9a1f114b6a5a107`  
		Last Modified: Wed, 15 Jan 2020 01:51:03 GMT  
		Size: 70.0 KB (69974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae8d73c31bd6bb443dd054e2ff7514c3f89f2252ad8f45b02d272a63de3194`  
		Last Modified: Wed, 15 Jan 2020 01:51:01 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f6925b94821214a339a1b91016498dab123d6a0f54b1289d79d3899a99fdf9`  
		Last Modified: Sat, 25 Jan 2020 04:19:56 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6febf931c78388861960b1a4712abf31aa8ae9827dc7855d9662f38737a6691`  
		Last Modified: Sat, 25 Jan 2020 04:20:19 GMT  
		Size: 194.0 MB (194008348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08438ec9e79121f2e7b67b3c2eb8c6ff32d7d9a9b580b156f7bafda22a43a71a`  
		Last Modified: Sat, 25 Jan 2020 04:19:57 GMT  
		Size: 3.4 MB (3439946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bbc766b556be88628a7ba65db74dc68ef2e06c9d79ac6a47c5037bb9d6fdbc`  
		Last Modified: Sat, 25 Jan 2020 04:19:56 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
