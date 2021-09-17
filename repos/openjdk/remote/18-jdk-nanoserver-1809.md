## `openjdk:18-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:0d0a481dee8a376c2d752560b76b8047a8999504a1c4d6e0608f552c040bfc00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `openjdk:18-jdk-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:f4a4abef328c99a8215bcf47c65a3452dc1f86f631c20b3cf3af91b41f3a9de1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289214126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b467d427067f368acd7cc938691d1e25969fecc601c3992fafd6a64bbb221f5c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 00:38:24 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 15 Sep 2021 00:38:25 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 00:38:36 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 15 Sep 2021 00:38:37 GMT
USER ContainerUser
# Fri, 17 Sep 2021 19:33:31 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:33:46 GMT
COPY dir:458fd0bba173a5f36490cb481279bcc2942e8513dff44d4cf4999733e3c894cf in C:\openjdk-18 
# Fri, 17 Sep 2021 19:34:12 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 17 Sep 2021 19:34:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:807d06303c39b2317729754a4c7ad6501e59c16ee464f8f671f9947774f62f72`  
		Last Modified: Wed, 15 Sep 2021 01:10:56 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353abb4dcfd1456117623d23e4be07d7d5c9e18c7ddea8dfb6225f99efa904b9`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6beb0bff60eb1dfb88e1010454b9aaf8f176f0d004a94fefdedb88d8e7e2a4`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bcb79c10ca3fae0a02ab85be6ab15af3a4ac4d7a0b8b54fd7a9c12cdd0b203`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 75.1 KB (75126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57b1aff54bbfc95746d48fc4f9d9afbb2f1f02e7d7006d7a7d6265ae52f9289`  
		Last Modified: Wed, 15 Sep 2021 01:10:52 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e50a8aa69983fb8e8d57ffc4731bd5e43fa5c8f9113104609ffb84a68a4369`  
		Last Modified: Fri, 17 Sep 2021 19:42:33 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a829edad8a9baf6f3e5f6cbb05101c6d452f4e6481ec2217fe18989c5f83fdc1`  
		Last Modified: Fri, 17 Sep 2021 19:45:45 GMT  
		Size: 182.9 MB (182913558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a262a13f35c983093fbd52b915c22d92ec524ea6b3b7376fa7a2c10a56b12fe4`  
		Last Modified: Fri, 17 Sep 2021 19:42:34 GMT  
		Size: 3.5 MB (3515057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b08aff0fb5ef884b0c170caf1e8149cebd045f5d971860dd2433db2ffb907fe`  
		Last Modified: Fri, 17 Sep 2021 19:42:33 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
