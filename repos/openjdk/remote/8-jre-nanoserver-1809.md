## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:8a28ca3b2effdc0cfcba94633e43125cddf274897af786fef200f161f18cd1e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:f1553be0c187a0cddc72dc5108a8e5b9c40bbe7530e2d7b1c1bbd0257babd460
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139746842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f72e05fbba4c460af2d127a9d3a1fb2a5a3bf816bbd069c7287f6051d918d5c`
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
# Wed, 12 May 2021 17:10:22 GMT
COPY dir:f730d49fd573406c508c5c18daca9d2bf81afd7c16f0b64747f54fe283bbc615 in C:\openjdk-8 
# Wed, 12 May 2021 17:10:40 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:7ac0b9364cf48665a2d325f33bb0e0e70699796b7d867afa958b33394f453754`  
		Last Modified: Wed, 12 May 2021 17:34:04 GMT  
		Size: 38.2 MB (38216931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e4f553b053b17f84025de7a8ab2a65cd152a965abb7d479f6042bd371f037e`  
		Last Modified: Wed, 12 May 2021 17:33:55 GMT  
		Size: 80.9 KB (80863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
