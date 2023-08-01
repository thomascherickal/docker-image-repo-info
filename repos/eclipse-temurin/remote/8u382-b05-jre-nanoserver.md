## `eclipse-temurin:8u382-b05-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a42169a597b2212ee045e64988d24aff7e908619ec32206d46ef0d84e8f7e4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `eclipse-temurin:8u382-b05-jre-nanoserver` - windows version 10.0.20348.1850; amd64

```console
$ docker pull eclipse-temurin@sha256:6f6061afaf32419bd0bff34010a30f5cfed9785b6bca00d17387dd1bf1369fad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.2 MB (160172199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1a9f389aa084fe69ee0b12e831449d84107b65b764248bf43d4cae7bc094cc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 22:10:51 GMT
SHELL [cmd /s /c]
# Tue, 01 Aug 2023 21:26:17 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 01 Aug 2023 21:26:18 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Aug 2023 21:26:18 GMT
USER ContainerAdministrator
# Tue, 01 Aug 2023 21:26:28 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Aug 2023 21:26:29 GMT
USER ContainerUser
# Tue, 01 Aug 2023 21:27:09 GMT
COPY dir:f24575d0fd9e2979f5a8010c202ec6d963a3eb3cd788517e3ab1d758c8e6ad81 in C:\openjdk-8 
# Tue, 01 Aug 2023 21:27:23 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:7f465130b9f76189f7500fc2d88617c379871634f9ee1262c63fef5be58c5d38`  
		Last Modified: Tue, 01 Aug 2023 21:32:46 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1a32770a86c2fcf24bf7ecf869188e13f92c6e20be6abbc9df3b4e53e9ae11`  
		Last Modified: Tue, 01 Aug 2023 21:32:46 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca0e70e92b81f0349615836e5543a538f28f57bf260ce06800783ae5afae6be`  
		Last Modified: Tue, 01 Aug 2023 21:32:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372a2b40b17d66123e441e7445ac460f2b8b752f70d6c16a154755551c91c16c`  
		Last Modified: Tue, 01 Aug 2023 21:32:44 GMT  
		Size: 77.9 KB (77898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04d5157aa37070cf3b484c56c3f7f5a23d50a97480de0bbaa5034db4acdac0e`  
		Last Modified: Tue, 01 Aug 2023 21:32:45 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5843cb86fd66467bc642f410139710ebc0576ccca3e84c32dfc29b0874793766`  
		Last Modified: Tue, 01 Aug 2023 21:33:16 GMT  
		Size: 40.0 MB (39970969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357c1370261873bd8d24fb78372ddf73006996483f523513af38edd106d0168d`  
		Last Modified: Tue, 01 Aug 2023 21:33:09 GMT  
		Size: 61.1 KB (61074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u382-b05-jre-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull eclipse-temurin@sha256:20a7c83ad2e82cd361ef7042739f3b4928c3092459cc8144345eb65dbb2ad1bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144518211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a01441ea1da0ce16d68da21ee884f7692c6334dfafa1a4db838b6200a9a35dd2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Tue, 01 Aug 2023 21:19:45 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 01 Aug 2023 21:19:46 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Aug 2023 21:19:47 GMT
USER ContainerAdministrator
# Tue, 01 Aug 2023 21:19:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Aug 2023 21:19:57 GMT
USER ContainerUser
# Tue, 01 Aug 2023 21:24:17 GMT
COPY dir:f24575d0fd9e2979f5a8010c202ec6d963a3eb3cd788517e3ab1d758c8e6ad81 in C:\openjdk-8 
# Tue, 01 Aug 2023 21:24:29 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:f1c8394d64f526dec4ca3b20eded3b04f3a527669ee1d94b1c3a10eb76c7c0f3`  
		Last Modified: Tue, 01 Aug 2023 21:31:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dab1f3820ee6e69eb56c90cb7b89474eb05e0c7373793a3b755cf008f36b85`  
		Last Modified: Tue, 01 Aug 2023 21:31:19 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7135c46d9193a51c931c7c64e294600786a8c378ba679d14808f41e4c512fc7`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d61f4df5c7e0aa60343496495b61390672968a9b62b6683a9321df9f99b4317`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 72.6 KB (72611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1739e988680aa09378fe65cb99374b0be5bfff70eef733bc756693f5546cd96`  
		Last Modified: Tue, 01 Aug 2023 21:31:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40b20b2b0167f8eda225b30b8d3ce7c868c01ae414f2b4a5ef8fdb48f635d05`  
		Last Modified: Tue, 01 Aug 2023 21:32:21 GMT  
		Size: 40.0 MB (39981215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5d7a3c6329e4babce7565b9c3546cc8c937c8b8b85a437874a7b06a1fa7fb9`  
		Last Modified: Tue, 01 Aug 2023 21:32:15 GMT  
		Size: 50.4 KB (50379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
