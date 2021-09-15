## `openjdk:nanoserver-1809`

```console
$ docker pull openjdk@sha256:a10eff6456eb269840cf7393f1f82bfa7c209f1970d81d6637e6d4888d3bb76c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `openjdk:nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:182c0a1a1c574d0328694d9c7fd8e91e24f85978137d752b921d8ded36eae512
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.5 MB (288489244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fc73fece8020b6bbf0e9ca8d79441a008fc92a81ac324159f320663c3821d0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 00:43:50 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 15 Sep 2021 00:43:51 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 00:43:59 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 15 Sep 2021 00:43:59 GMT
USER ContainerUser
# Wed, 15 Sep 2021 00:44:00 GMT
ENV JAVA_VERSION=17
# Wed, 15 Sep 2021 00:44:16 GMT
COPY dir:16139fd5761a261a0505c9fb2561cbcbf9614d8d2403d5d2b56478bd7a396d2c in C:\openjdk-17 
# Wed, 15 Sep 2021 00:44:28 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 15 Sep 2021 00:44:29 GMT
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
	-	`sha256:c113a6f5a2db4bae7622435241135dc24a1dfa887ad8e7d874abcba362cb8a5e`  
		Last Modified: Wed, 15 Sep 2021 01:18:35 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81534ad8acfeddc25ce6e00c5907793450c4fa5055eaa944121072219564f6b4`  
		Last Modified: Wed, 15 Sep 2021 01:18:35 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f681c1b4421a0c5a3d20f2a3afe35d39074db7911c648725625fed483363ed40`  
		Last Modified: Wed, 15 Sep 2021 01:18:34 GMT  
		Size: 72.2 KB (72250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aafa789caf2976737e1056dbc9b49e8a3e70d7dca67c06668b2e7a7069c8f3`  
		Last Modified: Wed, 15 Sep 2021 01:18:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a53e5d401d7fe5f0baee43f4d5fb1f280567af8a4fe7703c7a8b3919e4ff60`  
		Last Modified: Wed, 15 Sep 2021 01:18:32 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8284e57e6723c1409af926cb931b5e6ad12ec46a1505ec41c9d4e2f194c24c67`  
		Last Modified: Wed, 15 Sep 2021 01:21:40 GMT  
		Size: 182.1 MB (182099484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7514b6825eceff320b32219c3521b6995673fe9627317671a77c30af3829097`  
		Last Modified: Wed, 15 Sep 2021 01:18:33 GMT  
		Size: 3.6 MB (3606846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cbe934d0556ec388f176971806be83a3f32e6d30b03ad03630b8af1d42721`  
		Last Modified: Wed, 15 Sep 2021 01:18:32 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
