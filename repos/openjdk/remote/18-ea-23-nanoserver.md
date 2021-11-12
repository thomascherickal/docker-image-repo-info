## `openjdk:18-ea-23-nanoserver`

```console
$ docker pull openjdk@sha256:e1005c7608d0dbc8e11a1537e61ea66d5979988bf5ca250a1d629a10f304b313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `openjdk:18-ea-23-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull openjdk@sha256:da7096128ebae52f41c02448005e1e5159764dc4b361e53da1fad7eeaf92e94c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289897209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f73a2bd0f4ca86b27c36e63d1ebe4f50062b1d35389c3efe639f971ef952f314`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 20:31:55 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Nov 2021 20:31:55 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 20:32:07 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Nov 2021 20:32:07 GMT
USER ContainerUser
# Fri, 12 Nov 2021 00:19:39 GMT
ENV JAVA_VERSION=18-ea+23
# Fri, 12 Nov 2021 00:19:54 GMT
COPY dir:c57b26bdf71babe6ed388ceecc62ce05111a8ba92c56d7151cc8ab7c3fca177a in C:\openjdk-18 
# Fri, 12 Nov 2021 00:20:16 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 12 Nov 2021 00:20:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e60ec86b90e1492e0e0ed2cbebcf624990a34862e24207343fd85b84b3544c8e`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d97d878bac5dd9dcbe1bb5f45ade2111fc77e8d4a5a348163bd9c3ddddbaf0`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a46fd95d3a8e8b5949c49cc0d70b858bddbe38c8c33e0a6a3e0f157d7795a`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88539ad3f1fb0ea6957da9a7298c1f6546afbb52b2deb7199763195fca993d98`  
		Last Modified: Wed, 10 Nov 2021 21:11:37 GMT  
		Size: 74.2 KB (74205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d133fe2173015750539b2d0a8fb86dbdbe0c6b44c8d75ddeb714a82814f98e00`  
		Last Modified: Wed, 10 Nov 2021 21:11:33 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46325dff17f5b4239f66a13aaf7dbd7489127fdb7d94e5063152f5a4191914b0`  
		Last Modified: Fri, 12 Nov 2021 00:27:03 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc80676d2060c0cf6ad3d08a15974fe9d33c1407325ba3eb68e99f5bbdee8fc`  
		Last Modified: Fri, 12 Nov 2021 00:30:24 GMT  
		Size: 183.5 MB (183534009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e2c6fbe24c9914b0e4ab915a359a818b931a684e440c23f1df4920c41081`  
		Last Modified: Fri, 12 Nov 2021 00:27:06 GMT  
		Size: 3.5 MB (3499225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3f64c65e306fd4d054e85d2790dc02aa100011e1f05ded8bc1aa07d98061f0`  
		Last Modified: Fri, 12 Nov 2021 00:27:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
