## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:61fc9145f084547b7c8200e57bb43711406af2ccbc52b6e4e79f23d4dfdff520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:198180b831335c37e827187d6494b40d03fd9977315d8aa266e86cfdf0882ac2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160579117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bbf5c6d0b4dcbf4fce05e6d62a48246fe23229a5aef473fb8b0371fdc1c829d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:54:07 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 01 Feb 2022 22:54:08 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 01 Feb 2022 22:54:09 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:54:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:54:25 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:55:49 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Tue, 01 Feb 2022 22:56:02 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cb6dea87f405f4fa73fd6347557a3648da3dd84633c426503c1b7f14951429`  
		Last Modified: Wed, 02 Feb 2022 00:57:34 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a13818bbd58ec688e0ec495adddfae4b3d2bda8a31c04889a880303f5094980`  
		Last Modified: Wed, 02 Feb 2022 00:57:34 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3a81eca58abad00dc1c363be743f173bde6903520c269a60d9bb522a72bb9`  
		Last Modified: Wed, 02 Feb 2022 00:57:34 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2600b7a2ce0292c8f576022c07fd0008587c534c14f8eb4c50da0f1c1a611dfa`  
		Last Modified: Wed, 02 Feb 2022 00:57:32 GMT  
		Size: 80.1 KB (80110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3456a2554ddb4c83dc441c9b31481fc592cfdb5f94be0f93899f20ff0f192e70`  
		Last Modified: Wed, 02 Feb 2022 00:57:31 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9e316b85b16eb32823b089fdd4597e44374a1b9a09abae90a418355ea6a4c5`  
		Last Modified: Wed, 02 Feb 2022 00:58:13 GMT  
		Size: 43.1 MB (43103232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295c9d2c1a4397cfa0428bdda11ea1ea6d2588fceab4f15ac98946cf6c37f3ec`  
		Last Modified: Wed, 02 Feb 2022 00:58:04 GMT  
		Size: 57.2 KB (57247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:57dec7054a11d0b417cd52fe29ce5b87b37636fdc1d61d308932b8b54879c18e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.3 MB (149260783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1a06c5fbde3a050f053c52e32e957c06284239efba8929a29cf00174fe2748`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:44:32 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 01 Feb 2022 22:44:32 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 01 Feb 2022 22:44:33 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:44:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:44:48 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:50:21 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Tue, 01 Feb 2022 22:50:35 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa46078d43e189cb179b28360277a7a1b69c05506225c7766ae2b819c8a6392d`  
		Last Modified: Wed, 02 Feb 2022 00:52:39 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aa0019ebf2884a2d9814b7d62791e4ec33d23c9197b29fc9ecc254a88dfa02`  
		Last Modified: Wed, 02 Feb 2022 00:52:39 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dad7753aae33e006b182a2d844afa68565a9ef455182b6198ba1ed91da868e`  
		Last Modified: Wed, 02 Feb 2022 00:52:39 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdfff0cd0b8eec9f4e960a75c6be945ed4fcee89f1ca863d075cf40153f3a6`  
		Last Modified: Wed, 02 Feb 2022 00:52:37 GMT  
		Size: 68.3 KB (68330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6062a82b25b794141f784e0d97e33582e337b759a6b422159a15b9a164004b47`  
		Last Modified: Wed, 02 Feb 2022 00:52:37 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb6744500d5a2971fb5e8678f4cae8f9045425280300c92b28b19117c2b94e8`  
		Last Modified: Wed, 02 Feb 2022 00:54:16 GMT  
		Size: 43.1 MB (43109401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c54e6d28d2dbc7bb956598994be21855ec164c2834a92dd6ded3c91d23c861`  
		Last Modified: Wed, 02 Feb 2022 00:54:05 GMT  
		Size: 3.0 MB (3031205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
