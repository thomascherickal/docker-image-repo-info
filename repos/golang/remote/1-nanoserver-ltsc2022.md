## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:2c60ca86bd02743047d4c6b2eb5e36535a5c7353c7347a57dc8a33ecafb1d08b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull golang@sha256:9e65dfde725919e226db2558c9cb7f87130b2218fb0647a08c11a76292bfd0c0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.4 MB (267391272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df81b77750ad8915d8a74f7796d63344cc4979ebb9903424e61f5eee00128b9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Tue, 12 Jul 2022 19:39:12 GMT
SHELL [cmd /S /C]
# Tue, 12 Jul 2022 19:39:13 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:39:14 GMT
USER ContainerAdministrator
# Tue, 12 Jul 2022 19:40:04 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 12 Jul 2022 19:40:05 GMT
USER ContainerUser
# Tue, 12 Jul 2022 19:56:43 GMT
ENV GOLANG_VERSION=1.18.3
# Tue, 12 Jul 2022 19:59:13 GMT
COPY dir:f2d0f4a9267a591c33858aceb464994502f206b1bde0c83972e6f9e2e21fe641 in C:\Program Files\Go 
# Tue, 12 Jul 2022 20:00:07 GMT
RUN go version
# Tue, 12 Jul 2022 20:00:08 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:86ff096ef8c908f52d6e505ea5d69c2a28332387f40883a0d9a119dfbf999132`  
		Last Modified: Tue, 12 Jul 2022 20:22:56 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe23cc7fbe1bbfdb4f04675a25cad3444f0af01973afffe750e10ec965c72ee`  
		Last Modified: Tue, 12 Jul 2022 20:22:56 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde0d76670c26bd142f389e17d685a60ea3799ac70159e807e85edbaec29b888`  
		Last Modified: Tue, 12 Jul 2022 20:22:56 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5634d308ec110917e3cefa0c803d1a6d03a45c1579705e18d5982b22c64f7e46`  
		Last Modified: Tue, 12 Jul 2022 20:22:56 GMT  
		Size: 86.6 KB (86580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2804a718c3b2adb4f6ed1540e5545d671dbb8935188a6d8eaf82d8981f090b8`  
		Last Modified: Tue, 12 Jul 2022 20:22:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9714ebeacb1737a5b51afea42f9c456d30be2f70774d11a294abe53a72e08935`  
		Last Modified: Tue, 12 Jul 2022 20:27:23 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c360e699d68a213e179f413445e73625e824eefa9666b19a2a53aa28a26c52`  
		Last Modified: Tue, 12 Jul 2022 20:28:15 GMT  
		Size: 149.2 MB (149202521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d29c9699253b27c6dc8e3e16270a636555c881e0a8106065dc2b24b314fff`  
		Last Modified: Tue, 12 Jul 2022 20:27:23 GMT  
		Size: 48.9 KB (48932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3725ed10de28e7955f424826d259e3c264de262c9e6c3fa183a39964a2b7ce`  
		Last Modified: Tue, 12 Jul 2022 20:27:23 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
