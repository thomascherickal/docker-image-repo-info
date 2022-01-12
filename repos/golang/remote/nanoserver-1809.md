## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:4cb57172be473eb662acf9997b5d8552432c38e8e2e751e97078d5d697d84d6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2451; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.2451; amd64

```console
$ docker pull golang@sha256:cceafe8a17c592bf2193dd505a2e9f548aec0121338dfee32718d8e4bb5c9b35
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248250505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a4739f5fa9f40b3303d0c4dc512b8e45f1b22ab963dfd94f9bb56e35cc2e32`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Jan 2022 05:19:42 GMT
RUN Apply image 1809-amd64
# Tue, 11 Jan 2022 23:45:46 GMT
SHELL [cmd /S /C]
# Tue, 11 Jan 2022 23:45:47 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:45:48 GMT
USER ContainerAdministrator
# Tue, 11 Jan 2022 23:46:01 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 11 Jan 2022 23:46:02 GMT
USER ContainerUser
# Wed, 12 Jan 2022 00:05:56 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:08:32 GMT
COPY dir:7d325dd3c7e81bd29326c5fb7b320ff307098f97c2703658681dad899622f617 in C:\Program Files\Go 
# Wed, 12 Jan 2022 00:09:19 GMT
RUN go version
# Wed, 12 Jan 2022 00:09:20 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:f9d5f05eef69cdb907192f860ff14ce569d925f1f53ac5255a5b37631124fd4d`  
		Size: 103.0 MB (103014618 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32c0d1014d722d5ddf8a2cfd689d84c3d41526e917e4938b3b2d4c1cab54ff47`  
		Last Modified: Wed, 12 Jan 2022 00:36:54 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cea66350d03b24cd4fd20e14aaf4f118fe7fe57be89cd92b96d752a4f06eb2e`  
		Last Modified: Wed, 12 Jan 2022 00:36:53 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7acea54aacedd665d2cc995181199deccf7b9a57a1d69cd1aa571f0d54da2ba`  
		Last Modified: Wed, 12 Jan 2022 00:36:53 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0484494ec94d47af3fff7024332b3c3e7382e1ff90a647405f0f8224d2fc0f3`  
		Last Modified: Wed, 12 Jan 2022 00:36:53 GMT  
		Size: 68.3 KB (68271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10616ae6b0613dc9115455d64655579f8c309c2ecfa0149a841e373e515fc70b`  
		Last Modified: Wed, 12 Jan 2022 00:36:50 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4efd69723f27d6231784003c9b02cf534fe53056a368facd317a7845c3b411`  
		Last Modified: Wed, 12 Jan 2022 00:43:04 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebc3a4eb55755c4fa08f19fcb6789fb882f22d4d4bacfad121ca8ddd82d92b0`  
		Last Modified: Wed, 12 Jan 2022 00:43:37 GMT  
		Size: 145.1 MB (145092929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf901ad41b716d4d786bc71d8e29f74f0622c1db70af3c90e1dec8005e7742d`  
		Last Modified: Wed, 12 Jan 2022 00:43:04 GMT  
		Size: 68.0 KB (67985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e299ae0dd632559db7e5091f098e0f6e2f27fdc8a89bbb0bc786f73196a2d9`  
		Last Modified: Wed, 12 Jan 2022 00:43:04 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
