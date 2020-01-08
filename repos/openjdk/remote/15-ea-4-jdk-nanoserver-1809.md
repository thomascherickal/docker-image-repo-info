## `openjdk:15-ea-4-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:756411fb3bc1d8acd747dd62d2110a15055a153ae1357693fdd30dbf2b255141
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `openjdk:15-ea-4-jdk-nanoserver-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull openjdk@sha256:4a8573e3dcf0bd6e0d1b686f07011c4cf81dcdf508503993896381f4ac83f4a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298526445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0b337b44c83ab463d63da056e7715cdaff736c6e6d3c5f0fb481849d2a0338`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 28 Nov 2019 13:16:41 GMT
RUN Apply image 1809-amd64
# Wed, 11 Dec 2019 18:49:48 GMT
SHELL [cmd /s /c]
# Thu, 19 Dec 2019 01:29:02 GMT
ENV JAVA_HOME=C:\openjdk-15
# Thu, 19 Dec 2019 01:29:03 GMT
USER ContainerAdministrator
# Thu, 19 Dec 2019 01:29:15 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Thu, 19 Dec 2019 01:29:16 GMT
USER ContainerUser
# Tue, 07 Jan 2020 23:31:17 GMT
ENV JAVA_VERSION=15-ea+4
# Tue, 07 Jan 2020 23:32:18 GMT
COPY dir:83afa8f8ba97f8f7954d098b7288b36f82237e572f47d666b37c7504511161ab in C:\openjdk-15 
# Tue, 07 Jan 2020 23:32:45 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 07 Jan 2020 23:32:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1951f408509ba9ddcf240ef5d838c72c5596f97a05b063446508f2ba15d510f2`  
		Size: 101.1 MB (101106116 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:163d55b77f49371136083ba8066ddbec4afad6e1f4fbba77fa4ffebc99a8098a`  
		Last Modified: Wed, 11 Dec 2019 20:01:21 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63bb05b94288d5ea0447e7c6b75a854704f420c56d3b13acab4d9b2e03cc3f4`  
		Last Modified: Thu, 19 Dec 2019 01:38:08 GMT  
		Size: 914.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64927380268ba75b4d8445c6eebea564ad1af3f6ffcd0ab9856b348138b44532`  
		Last Modified: Thu, 19 Dec 2019 01:38:08 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca8bce76a22921ecaa2f6065834a3d494b61f569022c5b64bf0c9fa9c5bc63c`  
		Last Modified: Thu, 19 Dec 2019 01:38:08 GMT  
		Size: 71.4 KB (71377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b95fb661adc21f04050381ea3e21b42927fa5df24d3b78a394b6e71e7992c12`  
		Last Modified: Thu, 19 Dec 2019 01:38:05 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917eb2035c2e37a0c3aacb8953d8966923f3376af8f7c84e4a5dfbef13f558e1`  
		Last Modified: Tue, 07 Jan 2020 23:50:26 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3621f349317b187cb51485a6d5c94c0386d3fcd8a8e582ff43912434b034505b`  
		Last Modified: Tue, 07 Jan 2020 23:50:59 GMT  
		Size: 193.9 MB (193900362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4388142004aeb55484147dcab58fe6dc97b63ee2f8660fb0b198248621f7e4fe`  
		Last Modified: Tue, 07 Jan 2020 23:50:27 GMT  
		Size: 3.4 MB (3443005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f74ff38a97531fa90c866ab611f1e508b0082dbb31aa116a025a263f97ec30c`  
		Last Modified: Tue, 07 Jan 2020 23:50:26 GMT  
		Size: 908.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
