## `openjdk:17-ea-20-nanoserver`

```console
$ docker pull openjdk@sha256:6afa043d3edd0c005fe747c13883d4f2168f8a0edffc3292bdd29b27f2d00366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:17-ea-20-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:4ff4d549e378a11901e94642e3f65979b93a47f01af6263135c4340e1979cc9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.0 MB (286037510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307e2cabc977287b2ef940b7fe17f34e7bdfd51254f19dba813913b289bd0326`
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
# Fri, 30 Apr 2021 21:19:08 GMT
ENV JAVA_VERSION=17-ea+20
# Fri, 30 Apr 2021 21:19:23 GMT
COPY dir:8a26d6bfa0f72c1ba7ab3c8172c18e96e06e4d45d27da735c47babb0d880c6b5 in C:\openjdk-17 
# Fri, 30 Apr 2021 21:19:47 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 30 Apr 2021 21:19:48 GMT
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
	-	`sha256:be84104d24e0f7235a892153d6911d5d354ddf52ddbe297a2a7a95d9dd05e787`  
		Last Modified: Fri, 30 Apr 2021 21:26:21 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a198b512f7364b7e018f0ba8467a4c92851d2dd7bd1c0dcab2ee1e2929fa2ee`  
		Last Modified: Fri, 30 Apr 2021 21:26:41 GMT  
		Size: 181.0 MB (180985142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97896ef2d9be4069a755e6dff27d903b6c7062033c1c4f1a58954ca6e15903d1`  
		Last Modified: Fri, 30 Apr 2021 21:26:22 GMT  
		Size: 3.6 MB (3639611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab70a7a80328e8d62fa50c2be54c7b5a5727a372a7fce5924d5af5d97ff2dbea`  
		Last Modified: Fri, 30 Apr 2021 21:26:21 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
