## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:c59eab6eb5ff5d5dd6090fac5dc19bdc80305b0b22ce586796f83cf9a5d7e14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull golang@sha256:f59acdda0a868ab900cd610b3ce18477d30891a536fe59b07405048e606a955c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (234955105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47bba05103297af855e720c73e5fa9d70bdaebfe75d0d00c69f3559cb75bc2c`
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
# Fri, 06 Nov 2020 19:21:48 GMT
ENV GOLANG_VERSION=1.15.4
# Fri, 06 Nov 2020 19:23:44 GMT
COPY dir:4e2d5ce67fad51e9fa7a1bb7e4b8080b653b043b49d71cae8b6334eed1d5b569 in C:\go 
# Fri, 06 Nov 2020 19:23:59 GMT
RUN go version
# Fri, 06 Nov 2020 19:24:00 GMT
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
	-	`sha256:95ed241549f83a364d4391f9244ad71bd54926c9793b18c8180a8406c67a21ca`  
		Last Modified: Fri, 06 Nov 2020 19:35:15 GMT  
		Size: 861.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d3e3ff3521ab1cbb220ab54e02f598f9aca31df5d7a5bb8308f0795edffab8`  
		Last Modified: Fri, 06 Nov 2020 19:35:49 GMT  
		Size: 133.6 MB (133604723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0bc5bd4253cb90c1cf1faa7f47040812eba7659cdce9b5935ce15b4b7f95b7`  
		Last Modified: Fri, 06 Nov 2020 19:35:16 GMT  
		Size: 75.9 KB (75934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e4da059938b5b6e79d507c529ee1fa7b4fcb4a230ba7c573d24efdbbdf09df`  
		Last Modified: Fri, 06 Nov 2020 19:35:16 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
