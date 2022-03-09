## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:839c41344bb223d81f216bc1dd8c30b9546104c4c2ec1e674b384e6dc05ffe39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull golang@sha256:04efb71ca1d620aa0b45be7b10eaf3ef2634fc28d7e6dd55d404431277f7269a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262815121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e699ed88d972cd6674c4bea05c944e1e536fee8c67dc022d399cda3af69dac`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Mar 2022 04:50:34 GMT
RUN Apply image ltsc2022-amd64
# Tue, 08 Mar 2022 20:12:59 GMT
SHELL [cmd /S /C]
# Wed, 09 Mar 2022 13:24:44 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:24:45 GMT
USER ContainerAdministrator
# Wed, 09 Mar 2022 13:25:32 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Mar 2022 13:25:33 GMT
USER ContainerUser
# Wed, 09 Mar 2022 13:38:37 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:40:49 GMT
COPY dir:30287e5480cb94d00aba798bdf22cad49bb2ae2de25f97441d1d8401e0571f4d in C:\Program Files\Go 
# Wed, 09 Mar 2022 13:41:39 GMT
RUN go version
# Wed, 09 Mar 2022 13:41:40 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:dad81795ce109a7e20ebf80ad31925797ed97f9ba2a559f13f96ce3be5ea712b`  
		Size: 117.5 MB (117485491 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1c729ab19fa1794c04e2296ab2468daa560c676da6b333af3a86d94c1dc68b9`  
		Last Modified: Tue, 08 Mar 2022 20:39:41 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d268713d049d728054e11cf9c9306338ca1897c15a787ceafe9ee0fd8e305ac`  
		Last Modified: Wed, 09 Mar 2022 14:07:14 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcf1bdf8d65a7c4fcaf57246cc53c3f7f2aec0d0bdda306af3ab88084aa45b7`  
		Last Modified: Wed, 09 Mar 2022 14:07:14 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5fcf8d11464dbc6517a2f7808ad6c5c02360e3412d6b2881e9d61ef4eb3154`  
		Last Modified: Wed, 09 Mar 2022 14:07:13 GMT  
		Size: 79.5 KB (79469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55a006dc03085816dbdd7b07c4c2b36eeabf1dab04daec03901643c6461746d`  
		Last Modified: Wed, 09 Mar 2022 14:07:11 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54289a2ca518d735438266dd83750cbe06250ed2bfacd57f9caff0c2480c56f`  
		Last Modified: Wed, 09 Mar 2022 14:13:22 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8740521d551fe103d0acd182ff818d1a3675086d7eec9ffaa112292fb2a339b8`  
		Last Modified: Wed, 09 Mar 2022 14:15:55 GMT  
		Size: 145.2 MB (145192764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caee94a79c286bf31e55da47a8eda92fbfd32da85d892f469cbedcf5da68616`  
		Last Modified: Wed, 09 Mar 2022 14:13:22 GMT  
		Size: 50.3 KB (50280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae3d1b28a5a5d680ae1f631c590d7c117d986335482ad9b56ec233290a1e5c1`  
		Last Modified: Wed, 09 Mar 2022 14:13:22 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
