## `openjdk:11-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:b2c5b438591d488e27b8cda86df99537ae2ce23b738e0765ddaf9e097d4c3e2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:11-jdk-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:d467fe905850ae141193d0b2896095737d63b2762a15c0da6a6c1bd24186bb04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293923982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660e3255572fa58b370f962382b04e5200205a95619aa863ec326cf6aa3737d0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 00:59:21 GMT
ENV JAVA_HOME=C:\openjdk-11
# Thu, 14 Oct 2021 00:59:22 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 00:59:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 00:59:32 GMT
USER ContainerUser
# Thu, 14 Oct 2021 00:59:33 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 14 Oct 2021 00:59:53 GMT
COPY dir:8d687b3cc71690b95b3812413f66d278c1566215f055e8d2ed9ac022b638e9a3 in C:\openjdk-11 
# Thu, 14 Oct 2021 01:00:08 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 14 Oct 2021 01:00:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43342c8994cfe8e109320781e376005858ed6af7b5e15090c692a48ddee1c9d1`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf3a714ac5c06b6ff3556dd1e4f015c50841a0819a87a526dcbdc6dbf295478`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d5e43d0b80f79ad39e7b8a9d5f3b829595776b1abdf47c07fe87891d489583`  
		Last Modified: Sat, 16 Oct 2021 00:48:14 GMT  
		Size: 75.1 KB (75090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20aa72adc10eb6d0803d15b38f310dd050e3662bf077f683fea6ff85482f1a69`  
		Last Modified: Sat, 16 Oct 2021 00:48:12 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598cf4f37d35ab31fa8599a77460bcc5cb1668dc148d98ecfae391cc55ec80a6`  
		Last Modified: Sat, 16 Oct 2021 00:48:12 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b516797abdd52838554311e06058f2f8008a96439ce3f618cb06072851c35fd9`  
		Last Modified: Sat, 16 Oct 2021 00:48:31 GMT  
		Size: 191.1 MB (191124097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a733c272bcd3972de310f49d5f0f2ab8d92ae425f35f25631804eeeac03f8121`  
		Last Modified: Sat, 16 Oct 2021 00:48:12 GMT  
		Size: 56.6 KB (56559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4893c6a3f9ea6416825c4f913f5e46000adc3e5df66ea61e0d71c5376babbf84`  
		Last Modified: Sat, 16 Oct 2021 00:48:12 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
