## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:4d670dd2a11c6125bd298bbedd20b785634fb050b3837795a274d4d2e9f62921
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:101623d3531745b365e0102d6af720d58d97d6995c78c6c33e095a7b74e54962
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138559598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d9ab0968dab11e4321d55db00091e33bda974d04a8e8dca37d15d4c40c2b68`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 15:30:41 GMT
SHELL [cmd /s /c]
# Wed, 13 May 2020 15:57:11 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 May 2020 15:57:12 GMT
USER ContainerAdministrator
# Wed, 13 May 2020 15:57:23 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 May 2020 15:57:24 GMT
USER ContainerUser
# Wed, 13 May 2020 15:57:25 GMT
ENV JAVA_VERSION=8u252
# Wed, 13 May 2020 16:01:29 GMT
COPY dir:efe8678d9be4067f8f1280960ef457f634d7198257f7398711cb683e771f08bd in C:\openjdk-8 
# Wed, 13 May 2020 16:01:45 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c597e8fceaeb76628095f6dcfa538d497e85739068a817b45d73be2b96a3b37`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab776ab4b50d0cfd71683078381ed7262c0714503d1c51a1c1a17638582efb1`  
		Last Modified: Wed, 13 May 2020 16:29:15 GMT  
		Size: 824.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95de4896b5ed497cac9ccbb2ed31616aeade69a3c79b64b15196f19097b31500`  
		Last Modified: Wed, 13 May 2020 16:29:15 GMT  
		Size: 815.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d09afecfcc0bad842ec8f2307cdb919b3340e6af09ec581d45fcfd9f60d99`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 71.2 KB (71155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb3c5b23798be09045e18678d06d3941c514f0737db5afebdc8e7da58d7d08c`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059a1563d2f1af8c439c8c7d613fdd205e7beba82ffc15ee22d2ae3c37012f9e`  
		Last Modified: Wed, 13 May 2020 16:29:12 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b49e248c4ff2889cfb704ee4a2cb2e752ed3bec87649de4e87266c0a55384dd`  
		Last Modified: Wed, 13 May 2020 16:30:27 GMT  
		Size: 37.4 MB (37420902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f92f7d3de34276378213b4d86361af52aec7d684241eeca5778c5706c14590`  
		Last Modified: Wed, 13 May 2020 16:30:20 GMT  
		Size: 43.4 KB (43432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
