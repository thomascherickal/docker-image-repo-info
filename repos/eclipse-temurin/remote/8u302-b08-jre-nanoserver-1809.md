## `eclipse-temurin:8u302-b08-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:5c282ad74ce6b63178f673621420b1ec9067c9ceced7c322fc343f13a7e1eeed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `eclipse-temurin:8u302-b08-jre-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull eclipse-temurin@sha256:abad36e6e7ebca6e376712be0c4e18417fc64507487a0c04b5441bfe7dd75d04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.0 MB (203026364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2224a8e9921553223f75144e6a0977d4ef1ad690eb311d4b6d599ad048a4e68`
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
# Wed, 15 Sep 2021 16:25:47 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:8dff412359ba6bc290be26d16c45fca37b771fc28f6a332594ed8f88ad253d51`  
		Last Modified: Wed, 15 Sep 2021 16:44:20 GMT  
		Size: 80.6 KB (80573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
