## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:6054ba631cd86035b98e7c58896092631f014f37fe9efe065533262f2e8f519b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:1fffcc831806600b4ef36ec51df949f7f7051c732a489832e3e4cbbd2f3212dc
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.6 MB (200647855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acce24a5ebe53c09ce41c0619f6c95d04d122d65a4dfd6917648bf9286da0296`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jan 2020 23:56:11 GMT
SHELL [cmd /s /c]
# Wed, 15 Jan 2020 01:37:11 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jan 2020 01:37:12 GMT
USER ContainerAdministrator
# Wed, 15 Jan 2020 01:37:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jan 2020 01:37:26 GMT
USER ContainerUser
# Thu, 23 Jan 2020 00:27:00 GMT
ENV JAVA_VERSION=8u242
# Thu, 23 Jan 2020 00:27:47 GMT
COPY dir:604850e4892a2e6375b4d95fb378e9776042497a20a33de1bbe6b0d17fade1d2 in C:\openjdk-8 
# Thu, 23 Jan 2020 00:28:07 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:764e25aa4e95684bd69a4d130dc1c729bfaef95293d9c76c4d2a12ced9e3a9ac`  
		Last Modified: Wed, 15 Jan 2020 01:51:06 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b207e8571875b5c57f6bec51eea1e0fc14627b12fe76121e7a220c2870ec6c`  
		Last Modified: Wed, 15 Jan 2020 02:16:26 GMT  
		Size: 919.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb4e324b3232465d20aa50722eb8ddd36076bba06d7903391ea8b65d41fc3d1`  
		Last Modified: Wed, 15 Jan 2020 02:16:25 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb46126f2f094e1347e791f19d060913b307a75f7732fe94aeabf500c9ef057a`  
		Last Modified: Wed, 15 Jan 2020 02:16:24 GMT  
		Size: 72.1 KB (72068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0327ebcd1fd4b5d11809f5351b664cd79050fa966f08e3777e8b25082e3036`  
		Last Modified: Wed, 15 Jan 2020 02:16:23 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4908bffc2cb9ebfdae93b8e60b577950704818b181aa975c2b9a3e93a28f6c`  
		Last Modified: Thu, 23 Jan 2020 00:36:37 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fd722780e84b56f636ed2f220ced32786bd58176b7fad176cdff23d591f191`  
		Last Modified: Thu, 23 Jan 2020 00:36:54 GMT  
		Size: 99.5 MB (99475449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43abd03d1ffe0acc5b49df6d781bdd56a1bea411644f61d5bc0c1f6f69c4a911`  
		Last Modified: Thu, 23 Jan 2020 00:36:37 GMT  
		Size: 41.4 KB (41364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
