## `openjdk:20-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2085b73b74646936f7fde1290a37be5232d8f5843fe88a797874a19f751923d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `openjdk:20-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull openjdk@sha256:7a00dee940df2fbab63b70a13972ea062dd856c9032ee9f36a22679619353eb1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303883848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47871a4632bb5a5e617594d1c0b53272fda8e65bbd41e54ce8caa3cc2ef882c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Tue, 08 Nov 2022 18:36:25 GMT
SHELL [cmd /s /c]
# Wed, 09 Nov 2022 17:26:48 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:26:49 GMT
USER ContainerAdministrator
# Wed, 09 Nov 2022 17:27:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Nov 2022 17:27:07 GMT
USER ContainerUser
# Fri, 18 Nov 2022 01:18:11 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:18:27 GMT
COPY dir:230917fdc3635f9060cc2b8443084bd903740ea0631d84df0ba8941729313c5b in C:\openjdk-20 
# Fri, 18 Nov 2022 01:18:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 18 Nov 2022 01:18:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f4bb4b79b67857c1e4ac5c66026fd5ff5badbde5a8b59b11251b02699586`  
		Last Modified: Tue, 08 Nov 2022 19:44:52 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5380ecadb3b5072bd5e7cf41fa446b5ae89ef7d71fde34772d7b32062aca954b`  
		Last Modified: Wed, 09 Nov 2022 17:37:09 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19002dcea365821038023716e28374a8210ac45b5a63b539639130ad9b6bd8`  
		Last Modified: Wed, 09 Nov 2022 17:37:08 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc05d65ddfbc35592002f4ae7726cad3fa9b8777ac1f0cbb66bad8963c18cc7`  
		Last Modified: Wed, 09 Nov 2022 17:37:08 GMT  
		Size: 74.7 KB (74716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0517802e30312d5724623bf6cc9fe338f7330d522b267fad48ae4f85da52072`  
		Last Modified: Wed, 09 Nov 2022 17:37:06 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503ed98a75d6fa04baab60abb943da8c84f4c6d15ad50744100173f0ea2c7d5e`  
		Last Modified: Fri, 18 Nov 2022 01:22:08 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3b5b39095dfbd34dbe2811dfbdd3a3a4ea12d53e5217c501adae6b7f23e251`  
		Last Modified: Fri, 18 Nov 2022 01:22:29 GMT  
		Size: 193.3 MB (193288199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14e6515b3764a0fb9682ac20e9a24fabf6b9bbe096be80011d07e3abf8290c`  
		Last Modified: Fri, 18 Nov 2022 01:22:09 GMT  
		Size: 3.8 MB (3790810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da8fd96d7bbf8b018cbca71adc6623093692fd674b89f9eb96331fab325e64`  
		Last Modified: Fri, 18 Nov 2022 01:22:08 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
