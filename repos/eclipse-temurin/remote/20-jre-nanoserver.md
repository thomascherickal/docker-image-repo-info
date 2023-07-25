## `eclipse-temurin:20-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:b24405a99ee4414c00471739a4283339691892788692132fc2a88af08f05d13a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `eclipse-temurin:20-jre-nanoserver` - windows version 10.0.20348.1850; amd64

```console
$ docker pull eclipse-temurin@sha256:f2e041409b115ec1eca3d3a9d443aba13ca6ba9225c8f0ce3a1eb507f5985ba4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166051151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399e668bfcaf16fd7849058b4ddd8f69213c85d94262693ae5cfc9b20188f080`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 22:10:51 GMT
SHELL [cmd /s /c]
# Mon, 24 Jul 2023 22:34:58 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Mon, 24 Jul 2023 22:34:58 GMT
ENV JAVA_HOME=C:\openjdk-20
# Mon, 24 Jul 2023 22:34:59 GMT
USER ContainerAdministrator
# Mon, 24 Jul 2023 22:35:16 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 24 Jul 2023 22:35:17 GMT
USER ContainerUser
# Mon, 24 Jul 2023 22:36:08 GMT
COPY dir:7e69bb3960973ab39fc2ba0552343e70b32506a25a841e69600e9c49be1d11aa in C:\openjdk-20 
# Mon, 24 Jul 2023 22:36:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:cc0a26bd90fcc4d863317c36d7ffec77a0a82a905697204d4dcbc76ec13b3920`  
		Last Modified: Tue, 11 Jul 2023 20:10:45 GMT  
		Size: 120.1 MB (120056465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11750b624a775aa3c21a13406dfc54458855b8684e21efba5bbb9b27ee0b12`  
		Last Modified: Thu, 13 Jul 2023 22:28:35 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df03e5a85a6761fb9efe6df02bff339628d33192479fac4f4c80765ecb467eef`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb4d53565cdd7fcb858eea61889381d14090947f03297df736e4c9cb1eb0b0a`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b41305755dfc1b9134e1943811949039f0f83b9c472199fb2a1f87bb4fa648`  
		Last Modified: Mon, 24 Jul 2023 22:42:01 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfdf758fe560a8a115eed1641a54aa1d98588b326ed28c0f4f9ba9f13d2d528`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 78.7 KB (78687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610d1be704af1f3692c5ba787db39540820b0f50a7540e0e953478d58bf4414c`  
		Last Modified: Mon, 24 Jul 2023 22:41:59 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e002847964e0306277e9d3fb0491542d6856ceece2953aae8005cd90add3a4`  
		Last Modified: Mon, 24 Jul 2023 22:42:40 GMT  
		Size: 45.8 MB (45849073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f9c53db8f829d84afd66b6e58e88b4bc51aa3b93d3443e0129dc1e7c72347`  
		Last Modified: Mon, 24 Jul 2023 22:42:31 GMT  
		Size: 61.1 KB (61092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull eclipse-temurin@sha256:6441399d0738224e3f46f6318b11e585e4f84f0f67f96ec94ee863652ffbcb7a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153484195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415da472db1b30d43ed07b2c9fc4b26326bf9d8d008abc42061534a5b9942758`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Mon, 24 Jul 2023 22:29:10 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Mon, 24 Jul 2023 22:29:11 GMT
ENV JAVA_HOME=C:\openjdk-20
# Mon, 24 Jul 2023 22:29:12 GMT
USER ContainerAdministrator
# Mon, 24 Jul 2023 22:29:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 24 Jul 2023 22:29:26 GMT
USER ContainerUser
# Mon, 24 Jul 2023 22:34:06 GMT
COPY dir:7e69bb3960973ab39fc2ba0552343e70b32506a25a841e69600e9c49be1d11aa in C:\openjdk-20 
# Mon, 24 Jul 2023 22:34:17 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3304d99bb45bd396562f7f91d37af5a446d4889b089704dd94525f599a313b5`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a234201ab08724053de32e2bb25598862ec6eead6ec84376abe96d5f5bcceb`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced14764f8bc8c1a02eb2929b520cbd53bd6a49cb6f9126918c7c487b27966ba`  
		Last Modified: Mon, 24 Jul 2023 22:40:20 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1db76a566fe492ce96b9e5d4d6ec9ebffec2219c549c0f580ed3b301d86e49`  
		Last Modified: Mon, 24 Jul 2023 22:40:18 GMT  
		Size: 69.1 KB (69098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f620e23904692174522ca4e362d9121e805c30bd6744dc90a68dd2c5f72f6ff1`  
		Last Modified: Mon, 24 Jul 2023 22:40:18 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69835702ac2e7be2a51a0fe78d01a4a5f2103940df6325ed2a9791c80208ee0`  
		Last Modified: Mon, 24 Jul 2023 22:41:44 GMT  
		Size: 45.9 MB (45854178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c79cd8886f0d61fd58340617eb0c51a73a19f3477f57f64f5d78f829126d15f`  
		Last Modified: Mon, 24 Jul 2023 22:41:36 GMT  
		Size: 3.1 MB (3146927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
