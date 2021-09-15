## `eclipse-temurin:8u302-b08-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:b13dfff49b878413f1df86a57a09d40709c2febbfca4ac165d6ea85fc35b8add
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `eclipse-temurin:8u302-b08-jdk-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull eclipse-temurin@sha256:451979dd2a37322f0755c529adfbc5b98ee49902c75261cc30a50047a7d3dc0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.0 MB (203035330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094c9486ca0f3489d80fd1426be64c8f52733cf2cc8c84fbcd1086826178c9e3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 16:20:33 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Wed, 15 Sep 2021 16:20:34 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Sep 2021 16:20:35 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 16:20:45 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Sep 2021 16:20:46 GMT
USER ContainerUser
# Wed, 15 Sep 2021 16:20:56 GMT
COPY dir:6622177b1379d4d7267ebc9bc4d0bb013ea883bae36028c72b4045f7fa088598 in C:\openjdk-8 
# Wed, 15 Sep 2021 16:21:09 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:807d06303c39b2317729754a4c7ad6501e59c16ee464f8f671f9947774f62f72`  
		Last Modified: Wed, 15 Sep 2021 01:10:56 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731adde04ee2252ac27813d5925fb91867aafd70d505dd0ee8c779d2f0861b0`  
		Last Modified: Wed, 15 Sep 2021 16:39:35 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ef075850bd103418d66728845f5b683d117cc72dc9975a5e22cb86e28bee97`  
		Last Modified: Wed, 15 Sep 2021 16:39:35 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007e224b123b02b7892d0aa9f4caf5a7c478f7d3e9792c9f21aa93237bf5da8c`  
		Last Modified: Wed, 15 Sep 2021 16:39:33 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01989fb22d68a2c36e984344fc8dea4c076ab04d33fd563fd39da6048cb39`  
		Last Modified: Wed, 15 Sep 2021 16:39:32 GMT  
		Size: 67.1 KB (67119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987abbd4e696821e711d73f2dd27ceae2ccf2c0ae0d9478fa3422269b416f99c`  
		Last Modified: Wed, 15 Sep 2021 16:39:32 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e4e85af5a6b7877e699233aa0feb34db785873b96a3c1dc00ab4e9367a0a31`  
		Last Modified: Wed, 15 Sep 2021 16:41:17 GMT  
		Size: 100.2 MB (100169589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364f9ae8aa819f22a71886d0121d7aa5e92b053e8e1ddb8e5134699733718f70`  
		Last Modified: Wed, 15 Sep 2021 16:39:32 GMT  
		Size: 89.5 KB (89539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
