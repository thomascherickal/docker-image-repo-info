## `openjdk:11-nanoserver-1809`

```console
$ docker pull openjdk@sha256:94a77428d6e631d50ca60a45a44b181fa4d55893ae659fe103a670af032f3191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `openjdk:11-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:848059502bcfaf312c5cb1a93c3efd0de81c931851d381b6c3cae5e5f667f56a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292528946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcabc80fc18175b3b3d2e6bc0a9bd6e28822c9510c356c0699059a2b52b3cda1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 16:42:56 GMT
SHELL [cmd /s /c]
# Wed, 12 May 2021 16:56:58 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 12 May 2021 16:56:59 GMT
USER ContainerAdministrator
# Wed, 12 May 2021 16:57:14 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 May 2021 16:57:15 GMT
USER ContainerUser
# Wed, 12 May 2021 16:57:16 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 16:57:36 GMT
COPY dir:fc1da1b67a232358030ccafe9e40cca6d0f12faab32f5871879cc4fd6550b119 in C:\openjdk-11 
# Wed, 12 May 2021 16:57:59 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 12 May 2021 16:57:59 GMT
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
	-	`sha256:d0dd30de8961df429a63ed8deef7569e57f46088774bdb4834406de3fc593403`  
		Last Modified: Wed, 12 May 2021 17:29:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5b7252d65c8b5a2080e823f74ea540f5e3b8ae212918f07299cf8195399792`  
		Last Modified: Wed, 12 May 2021 17:29:20 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717870b79744d1cd54daccac6e80d38ad1cf2e39b8e166eb2aef9f33995a7edd`  
		Last Modified: Wed, 12 May 2021 17:29:20 GMT  
		Size: 69.7 KB (69698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923b3574e8c6f8b9e59d5f63ccafbc7e2374b68e6dd9d7f9b3ce6e04cfaa1362`  
		Last Modified: Wed, 12 May 2021 17:29:17 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340f2f3f4d223e7d9bea5f96d684ceeefb76e99b6b64169cb936401cae45b01`  
		Last Modified: Wed, 12 May 2021 17:29:17 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9385158b2d5ce32b7c0392f3d6306caf82c6719168d43d142ba808c3e76ea9d`  
		Last Modified: Wed, 12 May 2021 17:29:38 GMT  
		Size: 191.0 MB (190986239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e9e8c63c00350e768cc5afb8f118e1d2e7da2756bd2027cc67155e0283375b`  
		Last Modified: Wed, 12 May 2021 17:29:17 GMT  
		Size: 90.8 KB (90808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877a067d7d9492f57d5ed0a003770e1b3acc716c886ca997f789ac2ef14b62e5`  
		Last Modified: Wed, 12 May 2021 17:29:17 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
