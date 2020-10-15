## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:1876d569e22abb0f07e99c324d8891999ebd073eb06de43859294808cd09f9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `golang:1-nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull golang@sha256:9d339a5477d4ce7fecf16847722a6e8fa180e18b42f5d5b71a35be58f306a912
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235202198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c179a88f330b5311593143fa997569cf672b0a6208d1463d7267de9a6e442c69`
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
# Thu, 15 Oct 2020 01:21:50 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:24:00 GMT
COPY dir:b2adfa626edba88f8a594c97293f1c3e77da1d5bb72229d22d4906b07425c954 in C:\go 
# Thu, 15 Oct 2020 01:24:20 GMT
RUN go version
# Thu, 15 Oct 2020 01:24:21 GMT
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
	-	`sha256:f74b8b11eb2f02c177e11b5575af8487fb6e6be624f18f1e682d07124ef64a87`  
		Last Modified: Thu, 15 Oct 2020 02:06:50 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff33e40614a3e5a9f0d492c5446d478c6716e79fb02dba56df38d342eb452da3`  
		Last Modified: Thu, 15 Oct 2020 02:07:18 GMT  
		Size: 133.9 MB (133862456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43b056b4b0d8477e89b87a7c0f11d84b42c987efc5333dc2f0562e0f53c088d`  
		Last Modified: Thu, 15 Oct 2020 02:06:51 GMT  
		Size: 65.2 KB (65239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3306b285f0618421b5e3145c43b3c1ccc2f27c3e00140ad2d609567b0a14bd1`  
		Last Modified: Thu, 15 Oct 2020 02:06:50 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
