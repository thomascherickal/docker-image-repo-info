## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:27d3bed3778740d330c99bbb26c2ef8f3904e9bd10134251418f838adb90701d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `golang:1-nanoserver` - windows version 10.0.17763.914; amd64

```console
$ docker pull golang@sha256:3d4a6da6abbe7ab80218c1562081c6da77baecad7acb1c5c2df37d05bf47970f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230764650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2be649d3ab4980cbb912004042d761280a927f6c81a5790c4aff09b581f3ef3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 28 Nov 2019 13:16:41 GMT
RUN Apply image 1809-amd64
# Wed, 11 Dec 2019 14:11:56 GMT
SHELL [cmd /S /C]
# Wed, 11 Dec 2019 14:11:57 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Dec 2019 14:11:58 GMT
USER ContainerAdministrator
# Wed, 11 Dec 2019 14:12:14 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 11 Dec 2019 14:12:16 GMT
USER ContainerUser
# Fri, 10 Jan 2020 00:35:50 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:41:10 GMT
COPY dir:20c9256b92c607cb3dcbafbae3a2844e3e96af89ea01ee7ff6c03a3681bb80b8 in C:\go 
# Fri, 10 Jan 2020 00:41:27 GMT
RUN go version
# Fri, 10 Jan 2020 00:41:29 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1951f408509ba9ddcf240ef5d838c72c5596f97a05b063446508f2ba15d510f2`  
		Size: 101.1 MB (101106116 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ed50be68803a1ab01775438a7c7120859af6d862951623c1f839bdaa6e753696`  
		Last Modified: Wed, 11 Dec 2019 14:46:36 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786791c892d16706f420a92f8994d9cb9dc343a68a235810d4738fb18b5b5276`  
		Last Modified: Wed, 11 Dec 2019 14:46:35 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93c8bd55e94ad5cd979b6d8e5bfe17b35239d815d08e879be34c62922272fa6`  
		Last Modified: Wed, 11 Dec 2019 14:46:35 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a79e898660655d6a4f59bef4d09f764b9d9f3f0b894d1311e7ca15b63f97fe`  
		Last Modified: Wed, 11 Dec 2019 14:46:35 GMT  
		Size: 68.9 KB (68897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35926f80f163893204e3384b3d8c95501eca046a877f340df6f4b59e7a851d9f`  
		Last Modified: Wed, 11 Dec 2019 14:46:33 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dda530ce939ced756219ae87df9950d574e910893e4c4f65e6664c51d048fc`  
		Last Modified: Fri, 10 Jan 2020 01:07:37 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28459a0e721eff60a6865ae75470bc07fcea5e29edcb34d487c755a2b3f33e8`  
		Last Modified: Fri, 10 Jan 2020 01:10:59 GMT  
		Size: 129.5 MB (129546380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579f55a876065ffa6a36bc1447252002d8f401d6314d582dfb6ffd57827e3183`  
		Last Modified: Fri, 10 Jan 2020 01:07:37 GMT  
		Size: 37.4 KB (37412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d672827cb3f58c08ac8227c8acab56a9b20c75de4d795fe7a3c36a557b651fe2`  
		Last Modified: Fri, 10 Jan 2020 01:07:37 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
