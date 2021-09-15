## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a2a82fd9f9b9ceb3f4716f169501eb7452e714f9d64720c0284c51c532471a49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull eclipse-temurin@sha256:0c9d3574ca9788aed566c0ca15207d0b8dcd4ea4aaea3658f90f26950c3e7c76
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294712672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7ab18591c0a2d3bbcf7b06ba5e716f45c2026dda2b8dde94875bf654657a6c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 16:30:46 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 15 Sep 2021 16:30:46 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Sep 2021 16:30:47 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 16:30:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Sep 2021 16:30:55 GMT
USER ContainerUser
# Wed, 15 Sep 2021 16:31:10 GMT
COPY dir:4c789b050c2a81313b7828df90f0ac6231d2beb7f7e21c1b81eca114d601d1fd in C:\openjdk-11 
# Wed, 15 Sep 2021 16:31:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Sep 2021 16:31:23 GMT
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
	-	`sha256:b4f0b46abc08dd348231f30302591eb106f2509c46e439c7735e18ffc04a3745`  
		Last Modified: Wed, 15 Sep 2021 16:51:52 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e03a155046076cc9ecbc1c5926012b18963df9b9df8ba86ff3ae4fb54efbbf6`  
		Last Modified: Wed, 15 Sep 2021 16:51:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fdd1cbc2a15e3bb42a7a8c1a542472bcbd16a3c372e40cf219996050315fa3`  
		Last Modified: Wed, 15 Sep 2021 16:51:52 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9056cfe69fb43064c5f5849e7f4328d6cffb416bfa2fdfc39b124fcf2f4cdce0`  
		Last Modified: Wed, 15 Sep 2021 16:51:50 GMT  
		Size: 72.3 KB (72298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a8abfaee4320d08e0142a1a43aa4330b43ed44f42af47dde036d39183459e`  
		Last Modified: Wed, 15 Sep 2021 16:51:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841b61345bf1fb409ab8a5e49480cc046cbce8b8987db2397ad7bd16ee123290`  
		Last Modified: Wed, 15 Sep 2021 16:52:06 GMT  
		Size: 191.9 MB (191880425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a27ddaf43c999f93a1a5ef031348ded9eb76c94b9495796c4231b6bf182f0e`  
		Last Modified: Wed, 15 Sep 2021 16:51:49 GMT  
		Size: 49.3 KB (49292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71506d9c7b35c62cc67fa617e8f6c3e34f0d0084537b13d3d559da54618ac4`  
		Last Modified: Wed, 15 Sep 2021 16:51:49 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
