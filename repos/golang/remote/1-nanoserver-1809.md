## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:1dbf2df7c6dce6674cd45219f98af85d327fd067eab5e26a86ffe72581315116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull golang@sha256:fac8f621ad160bc9433f5e067edb90c15b869354964501747636ea74e4a43171
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260809272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3a9b5b91934a9158df89ecac1f2ba08177dc5f45588e999c8093dba524de26`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 12:55:53 GMT
SHELL [cmd /S /C]
# Wed, 12 Oct 2022 12:55:54 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:55:54 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 12:56:23 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 12 Oct 2022 12:56:24 GMT
USER ContainerUser
# Wed, 12 Oct 2022 12:56:24 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 12 Oct 2022 12:58:53 GMT
COPY dir:1fc645e1b9a8ffb5757805e06eefa6c9c9b0f649b5403eeab554ede8594c418b in C:\Program Files\Go 
# Wed, 12 Oct 2022 12:59:35 GMT
RUN go version
# Wed, 12 Oct 2022 12:59:36 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:5ead999142ecce15e02523c49706a633fa708374d94bb65a254e3a3c117d609b`  
		Size: 103.4 MB (103377244 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3724c0f91ae729d3a2ed4ebab42f44a8e6cc1551989d86671030e217845bb6f0`  
		Last Modified: Wed, 12 Oct 2022 13:18:10 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a8c280073935e93a2c517be655b22a46ff381323f3dfbfb6c727bc3c3ceca5`  
		Last Modified: Wed, 12 Oct 2022 13:18:10 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c038a2fdb0b5bf749f14975c15563e9dfdd217a82aebcfe86eb523248a95851e`  
		Last Modified: Wed, 12 Oct 2022 13:18:10 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b094a8f8473a29ccb89c572abe211ff7acbc051960dbe7ad5ea518eda7550f9`  
		Last Modified: Wed, 12 Oct 2022 13:18:10 GMT  
		Size: 68.9 KB (68891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce65873524d60413e0be37057793d99214a7158eaebd8b2d6f1f377d5347a831`  
		Last Modified: Wed, 12 Oct 2022 13:18:08 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a092c9391f7b2dad402a37d614a00441a36400b4e4411ea82a8eeae616a79`  
		Last Modified: Wed, 12 Oct 2022 13:18:08 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5c9126ee730c9a5adb59b9b4f2c043e1c4b0fcbffbeaba6ce4f55137c80c93`  
		Last Modified: Wed, 12 Oct 2022 13:18:47 GMT  
		Size: 157.3 MB (157279751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e756884bcc31861bea03475d0d2299abbdff6c9f32be574b8cc4122ca10aa4b`  
		Last Modified: Wed, 12 Oct 2022 13:18:08 GMT  
		Size: 76.3 KB (76265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cae94f113eb0ac0cbdd672d316f9c524782897876c37583fea140ab11f4d93`  
		Last Modified: Wed, 12 Oct 2022 13:18:08 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
