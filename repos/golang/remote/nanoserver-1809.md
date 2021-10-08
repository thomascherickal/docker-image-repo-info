## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:9e558fb116aafdf20b0bec241feee65875d16729d231a5c8bf0918402f7fedc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull golang@sha256:bfe49faf9f3ea4ff0b44f073d97423234583551ad7477be9a467a0ee10f27368
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.9 MB (247931997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37f0c97defe057e486637eb55ded4c320f90bc5d550c505c4354965bd6f6b72`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 12:38:36 GMT
SHELL [cmd /S /C]
# Wed, 15 Sep 2021 12:38:37 GMT
ENV GOPATH=C:\go
# Wed, 15 Sep 2021 12:38:37 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 12:38:47 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 15 Sep 2021 12:38:48 GMT
USER ContainerUser
# Fri, 08 Oct 2021 00:29:57 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:32:20 GMT
COPY dir:9ade0ec1568a8830be528daab1970987eabfd3bd64d6ae74a94996a5d45cbeb5 in C:\Program Files\Go 
# Fri, 08 Oct 2021 00:33:06 GMT
RUN go version
# Fri, 08 Oct 2021 00:33:07 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2ca4d60596cfd2b5f14d3690345d5a3c729f5c92997c02dae42415488ac1008`  
		Last Modified: Wed, 15 Sep 2021 13:05:07 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440629e3e164571aacd603b2182b9c247d507467bdb083817c346bbbb6513973`  
		Last Modified: Wed, 15 Sep 2021 13:05:07 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7c8f44cbbaf6c8b375a2783723913bfbf53a33513d439811e785ae46e6f1e8`  
		Last Modified: Wed, 15 Sep 2021 13:05:07 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb48885a5ccaf9c8d8e69f3bb0fd77403366bd884a889408ded8ab83ba6172c`  
		Last Modified: Wed, 15 Sep 2021 13:05:07 GMT  
		Size: 68.1 KB (68085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c1d51e92ca574e622d8d830a48d878a457668e59fe5caebc43ff725d80b40c`  
		Last Modified: Wed, 15 Sep 2021 13:05:05 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d54d3ca2f3af7b322da554f4d2f674f3461710d236a370cba79b2a353111a7`  
		Last Modified: Fri, 08 Oct 2021 00:55:37 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e199fcb5f8d2495e675209361163eb660d4e6235048824805cdbce3c0d90e00a`  
		Last Modified: Fri, 08 Oct 2021 00:56:11 GMT  
		Size: 145.1 MB (145078940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837d62db07f802e65e65601946a1e6e0a7952b39e76b30f421646745913e89c1`  
		Last Modified: Fri, 08 Oct 2021 00:55:37 GMT  
		Size: 74.5 KB (74462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0ff90d371baab74927d58282e400f38a87edf473a57f13c90ac47b053c9ec`  
		Last Modified: Fri, 08 Oct 2021 00:55:37 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
