## `openjdk:8u292-nanoserver-1809`

```console
$ docker pull openjdk@sha256:308a57c9fcf0900db155b8362fda8019010164d3fe8db30d7d9532d679834141
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:8u292-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:50be09a1e8b9b7ab902e92c4b86c6a16c48ffd74731633d305ed638966306c39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202578698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6ed95b6ad39d330d43f428ece37b8d7d48c3568e73a69a52f8a25da71b8b74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 17:06:48 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 May 2021 17:06:48 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 17:07:03 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 17:07:04 GMT
USER ContainerUser
# Wed, 12 May 2021 17:07:05 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 17:07:21 GMT
COPY dir:04533fde1b9ea0cd60bd0fd48d2f644dab91f29f3b0d8a376770cc16b38c53d2 in C:\openjdk-8 
# Wed, 12 May 2021 17:07:41 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea91a7775c05d55a850a2983043468ce6ded7406743836cf8f33afb037aba1a8`  
		Last Modified: Wed, 12 May 2021 17:16:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb0862d58b0d0b43fc2ed0e7a5766f81e6c7b87623ae0e4f70b1b9be30fd9f5`  
		Last Modified: Wed, 12 May 2021 17:32:42 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2193e03a2055e1990834e75bd688f9250314f25c9d709e40fed0a9efe5814a34`  
		Last Modified: Wed, 12 May 2021 17:32:42 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183f4dbdb119d9dd765c24b150888c0396f759615485614016e5ee415b00d36b`  
		Last Modified: Wed, 12 May 2021 17:32:40 GMT  
		Size: 68.1 KB (68072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45067025d76c96ca9579808d88f84bf3bbe664f09da4668188d87b5d12ed7802`  
		Last Modified: Wed, 12 May 2021 17:32:39 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf425ef2f7296409dad08575f327774323f3df93a15ee0a39d3b2b26e40ff7f7`  
		Last Modified: Wed, 12 May 2021 17:32:39 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be372af847fad1d0b318ea5b4947f2e837ca5ee7456ac15f547803070be02cc`  
		Last Modified: Wed, 12 May 2021 17:32:58 GMT  
		Size: 101.0 MB (101039587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d56b7e95c41de0ce815d5c67f699b5e7348a10730f0b17fffc08524a163341`  
		Last Modified: Wed, 12 May 2021 17:32:39 GMT  
		Size: 90.1 KB (90063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
