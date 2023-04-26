## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:3597afbfc0bbd3924d1594ae4df20fe78aaf2317f64e4ee3fbb429647773b71a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull eclipse-temurin@sha256:58704cf2bc3d656904ad15ea4156657915fa24c4976f3d0b326a9b11f17b8b32
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165656552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f47065f9de2abb7df304679f33f4f2a85c906dc0b0761ecc27efaa75aa80d3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 01:42:21 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:53:33 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:53:34 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Apr 2023 19:53:35 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:53:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:53:44 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:54:24 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Wed, 26 Apr 2023 19:54:35 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8058ec80ac2516d001291dea383d4abfa22416397a4c869e6fd79c0d4b64565f`  
		Last Modified: Wed, 12 Apr 2023 09:45:40 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541dcd04867d15d0206d4505a5d5b19fff1e6d7d60f5495af08e9a2021d2a03f`  
		Last Modified: Wed, 26 Apr 2023 20:10:16 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f5b45aabda1fc50604908fc487e6166b8f81804b15b2c89f596c42dcc77616`  
		Last Modified: Wed, 26 Apr 2023 20:10:15 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7feee593188c152ce7a3ca060aaf7e884b20dad4552d8315f9d83d088ef8db1`  
		Last Modified: Wed, 26 Apr 2023 20:10:15 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b88778b47a0c3c2f257362fe2c2d39371d0a8c0ee7bb219f5cf9b457391ddb2`  
		Last Modified: Wed, 26 Apr 2023 20:10:13 GMT  
		Size: 83.9 KB (83868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c27b2cd5e9fb2782e4d60e6f9c99f77e3cb90286195338109b6b98ff3ba48d`  
		Last Modified: Wed, 26 Apr 2023 20:10:13 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79c806f662a395eeb6f8680699cf4d4867f5d3c196a9b73bd90c6dd166cc429`  
		Last Modified: Wed, 26 Apr 2023 20:10:51 GMT  
		Size: 43.2 MB (43163806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415460edad44a5f3dd5477b40860deeb661d3a31636a106a7df13be07f4d0505`  
		Last Modified: Wed, 26 Apr 2023 20:10:43 GMT  
		Size: 74.3 KB (74284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
