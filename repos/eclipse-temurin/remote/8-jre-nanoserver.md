## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:07352fd51b47cdefb7bd0c9bb35cd654993b335fda18f1c2e005070de91f9734
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:24689e8feb18dfe2072713d189fdb949ada7cd7d30bfbfc1d5a8def6c6e499f2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.8 MB (156839158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76ec4c27adce3cc6119824179c378490faa6d89ea3da9db4b4f7196ae65ef55`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:47:59 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:48:00 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Apr 2022 15:48:01 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:48:09 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:48:10 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:48:40 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Wed, 13 Apr 2022 15:48:50 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:924a7c42e559a85c0bc74dbb028ddeee43fe67b0f59c81c60cbda0082e0e3ae5`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165c132f9b7a99d82c74c6e8ae2683134d8e6f6668c194c6d67227d4f15f0921`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be478e3d24da72d6160915d7d5d8cf5a0eab20bcbb291144533fc87aaa32f0d4`  
		Last Modified: Wed, 13 Apr 2022 16:38:30 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a40a1449530555cd30b19c0d58a8e8e0938e6bf3f12ef294d872872114d4fdc`  
		Last Modified: Wed, 13 Apr 2022 16:38:28 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e54c826a7bf34947d87d543ed9b1b357b3c724a7b29bbb32d5c4d4126874f`  
		Last Modified: Wed, 13 Apr 2022 16:38:29 GMT  
		Size: 85.1 KB (85101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed1f47e5ce93097a6029a4c86ff2abc093cb444ec2ba87a93842307b0aa671c`  
		Last Modified: Wed, 13 Apr 2022 16:38:28 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69b7ccee87a15e8a0c8ec5b5a409d033694d71fcfdafda90ba6ed20f5cdd7d2`  
		Last Modified: Wed, 13 Apr 2022 16:39:34 GMT  
		Size: 39.1 MB (39107985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ccc35601dbd3f04f5e037bdca83dff81eb4c175860f1866833518f5abe7cb2`  
		Last Modified: Wed, 13 Apr 2022 16:38:53 GMT  
		Size: 61.4 KB (61375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.2803; amd64

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
