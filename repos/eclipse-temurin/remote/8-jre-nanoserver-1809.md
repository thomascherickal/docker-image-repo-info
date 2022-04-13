## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:6236465d2cad61df5edb6bd85944a2fdd1f6f39915b6461efe9dc48fb430aaa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:91b179e9a44e44d93402d741c4cedf92812233f9d4794903e3bc414c79b4c1eb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142338682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63639d707d09cc30fc3c0c621ce2ea0617c755c12fbe863fd188321ad1c32190`
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
# Wed, 13 Apr 2022 15:20:07 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Wed, 13 Apr 2022 15:20:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:c30f91bd926a51333891182026b31fad4c312e9482c41e6213b28c8a583d058b`  
		Last Modified: Wed, 13 Apr 2022 16:02:19 GMT  
		Size: 39.1 MB (39107510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46212136e558e1bb64e0cbaea811e5fbf6760ff742913cf14041a297cd8256f`  
		Last Modified: Wed, 13 Apr 2022 16:02:13 GMT  
		Size: 59.4 KB (59414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
