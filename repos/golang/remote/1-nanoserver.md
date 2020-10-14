## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:7b2dc9a5d2580553ec7687f18eb24b7aa7a17db0a59f8f71fe17a766f6360d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `golang:1-nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull golang@sha256:c303545373a79aa1cbbf1d46b36071de49f8237d3aba472ba44a5cbbe99efa82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235300168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16bca6844eba4aaae39f1bf60e0c701b74df8bdfc4474231a915fcc47dbc4a2f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 12:38:45 GMT
SHELL [cmd /S /C]
# Wed, 14 Oct 2020 12:38:46 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:38:47 GMT
USER ContainerAdministrator
# Wed, 14 Oct 2020 12:39:03 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 14 Oct 2020 12:39:04 GMT
USER ContainerUser
# Wed, 14 Oct 2020 12:39:04 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 14 Oct 2020 12:41:00 GMT
COPY dir:c68fd448135b1d496d0acfdaf09d10b1fbe646bd56bcd50e62788e87c715c4df in C:\go 
# Wed, 14 Oct 2020 12:41:15 GMT
RUN go version
# Wed, 14 Oct 2020 12:41:15 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5bc5109798f9a64116d8a878ce7b6065052706b8c0b20c2a60b08b6e159c98e`  
		Last Modified: Wed, 14 Oct 2020 12:52:17 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafbe105d874d1fbe9e0fdeaf9ced80d1b329d64e625ca269d104da231172923`  
		Last Modified: Wed, 14 Oct 2020 12:52:17 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f673d5ca3472f4c6af7b30975b97a04332942488339178e59512529f59cc5`  
		Last Modified: Wed, 14 Oct 2020 12:52:16 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6795e4c9fee91197bdf4d5305aa40977ab190c28a2d00b552f7e6affcbc3afa`  
		Last Modified: Wed, 14 Oct 2020 12:52:16 GMT  
		Size: 63.8 KB (63833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b552b565244b662f10f85146a0f2db636e34eb7d35caefc3761eb954693138`  
		Last Modified: Wed, 14 Oct 2020 12:52:13 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20585436fdf25a8cc500f777ba43219dee2fea2c757a2655d9b44068b67d6ec0`  
		Last Modified: Wed, 14 Oct 2020 12:52:13 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b8be8fb0be36bb598211644f2a5767764adeb4101acad71b615f43be0fe019`  
		Last Modified: Wed, 14 Oct 2020 12:52:40 GMT  
		Size: 134.0 MB (133954470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2062a81feea2bb6b1dc14f9b3d65985663d9a828eaf1b81fa1ec7b79c1db0fb8`  
		Last Modified: Wed, 14 Oct 2020 12:52:14 GMT  
		Size: 71.2 KB (71244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3de58b81c32aea61bb14453c0d52a29aeef916a9ee750cf588c14dfb76a6de`  
		Last Modified: Wed, 14 Oct 2020 12:52:13 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
