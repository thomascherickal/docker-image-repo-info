## `openjdk:17-ea-18-nanoserver`

```console
$ docker pull openjdk@sha256:a3ee3fe89dcbcd3a256a5cd92af454c9d3f7bb964515ee71e8a1720d13366ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:17-ea-18-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:9836775e3cec11009e4fd024350e22ee21acb8e54c3c51869e57dba38f00a481
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286107301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7b5f9b01de9f4e964a58807ca1c910506dcc521500f9420d6a9551f9a6b75a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:53:40 GMT
SHELL [cmd /s /c]
# Wed, 14 Apr 2021 16:53:41 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:53:42 GMT
USER ContainerAdministrator
# Wed, 14 Apr 2021 16:54:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Apr 2021 16:54:03 GMT
USER ContainerUser
# Fri, 16 Apr 2021 22:19:30 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:19:49 GMT
COPY dir:2a3262f093fae24e2f74445128d7d9aad89e29d74ef074d7a16b7239d3eb8281 in C:\openjdk-17 
# Fri, 16 Apr 2021 22:20:17 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 16 Apr 2021 22:20:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c2c727299531adc7c2aacb1f062d72fd42cec96a0d235b3e5b0afe03e9ddbc7d`  
		Last Modified: Wed, 14 Apr 2021 17:41:13 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4846a68a532c85058f47e1e9b777bab26eb5ad132cdeb3d646bc51d43346f1f8`  
		Last Modified: Wed, 14 Apr 2021 17:41:12 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede727741920ec94cb8aac2b231667fd531dbedb64b47f6dddc1577123fcd85`  
		Last Modified: Wed, 14 Apr 2021 17:41:10 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be7a926f02c08c32de5bc4e57d18923e0441090bd084aeb1b7dafaeb4ece58`  
		Last Modified: Wed, 14 Apr 2021 17:41:09 GMT  
		Size: 65.7 KB (65686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f5a6de061f5f5be316a0cf2d8471cf2baf8b3927a20b9d29826dc97bef2e54`  
		Last Modified: Wed, 14 Apr 2021 17:41:06 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee194119b78b06d727075b7e8b1ef8b56f030d88d7866734efc609648b09f2`  
		Last Modified: Fri, 16 Apr 2021 23:23:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7615fd49106a963d3e8eb13f277cbe67ac979d16ac1c027abe2fa0ed2f200a`  
		Last Modified: Fri, 16 Apr 2021 23:27:12 GMT  
		Size: 181.1 MB (181061270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e038a5b35a93ca976eb93e49b8491a628d0f22734a14f1cdfd5c6196f82199`  
		Last Modified: Fri, 16 Apr 2021 23:23:41 GMT  
		Size: 3.6 MB (3633242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f375203215d1000c8eee3ff0f92993939733af0ccf31441921d87542400fe90b`  
		Last Modified: Fri, 16 Apr 2021 23:23:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
