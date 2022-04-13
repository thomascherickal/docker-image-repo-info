## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7ca95e4f2e704e553996096122d6125e7556bfd913a3dd21b243aa56eb37c125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:465e1bf9d48719f5d785e504dfa708e7c741d4a5be63031e4452fddc5ab5cca3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203445392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf5f622f46187290895a43402f1a647599b61e387f05a0c531edce29c63d5c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:16:11 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:16:12 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Apr 2022 15:16:13 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:16:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:16:21 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:16:30 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Wed, 13 Apr 2022 15:16:40 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da95be465ebb87c1d8159ce71e30733274ed28cea4c1d8f2b5f9f4fb48549f0`  
		Last Modified: Wed, 13 Apr 2022 15:58:05 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b118ba79ffd3426bd8e686d11afdad0504c22cfaedba92c64b37a54ea404b9`  
		Last Modified: Wed, 13 Apr 2022 15:58:05 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d4915cf194433ec0b52e56a6e201cc17f0c17371020eac3f271b82f31c7252`  
		Last Modified: Wed, 13 Apr 2022 15:58:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e94414746f2588344400e5ea7a5b7824f3aed4329b02cb141cb4b22c1393c4e`  
		Last Modified: Wed, 13 Apr 2022 15:58:03 GMT  
		Size: 70.3 KB (70277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee992f632d4abe04da735089faa3e848ca43010143b86d28ff366b2d48f0fbd4`  
		Last Modified: Wed, 13 Apr 2022 15:58:04 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f4fe102c842baec32047d485727786920d943d10e922bc50819e818f6007c8`  
		Last Modified: Wed, 13 Apr 2022 16:00:13 GMT  
		Size: 100.2 MB (100214723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a705cdcc1f3e9f349f78da448815024432c6763219bef98260f60a08d9b0bbb8`  
		Last Modified: Wed, 13 Apr 2022 15:58:03 GMT  
		Size: 58.9 KB (58911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
