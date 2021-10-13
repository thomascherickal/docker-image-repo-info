## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:1443f72453a0fdabd6e9ff589ec92c5c500af7b114ea3fb50e34379a2b5a9ba1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull golang@sha256:4e76fb863d09e88e21974094e635b9a4dd4a7060e240e50f824b53cc53b0162b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.1 MB (262147233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0dfaffc9c566995652689cc2a461108f975a5564a8a1c458098c28af00df72`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 07 Oct 2021 11:15:04 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Oct 2021 12:48:50 GMT
SHELL [cmd /S /C]
# Wed, 13 Oct 2021 12:48:51 GMT
ENV GOPATH=C:\go
# Wed, 13 Oct 2021 12:48:52 GMT
USER ContainerAdministrator
# Wed, 13 Oct 2021 12:49:42 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 13 Oct 2021 12:49:43 GMT
USER ContainerUser
# Wed, 13 Oct 2021 12:49:44 GMT
ENV GOLANG_VERSION=1.17.2
# Wed, 13 Oct 2021 12:52:20 GMT
COPY dir:9ade0ec1568a8830be528daab1970987eabfd3bd64d6ae74a94996a5d45cbeb5 in C:\Program Files\Go 
# Wed, 13 Oct 2021 12:53:14 GMT
RUN go version
# Wed, 13 Oct 2021 12:53:15 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:91284e7e8fd4bd7ebcfa98544a3e4f59639f38281225c81c34b6fe22e0dba4e5`  
		Size: 116.9 MB (116939483 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:20e7750a023cb83652c7a9fb1fa59842126978ee34af47a4d3ed0508abf4b266`  
		Last Modified: Wed, 13 Oct 2021 13:28:53 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823dac1744a93be130acef2018641dda84d663debf8462412c9904299eed4bdf`  
		Last Modified: Wed, 13 Oct 2021 13:28:53 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3069ffd7a6649bf4acfceddd27a7177a71566770ca5e5aecbfe8daee26a6f1`  
		Last Modified: Wed, 13 Oct 2021 13:28:52 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0226fc2bbb1dd690934fb2d69ed72106e4b21592b4edb1d373d14d7e7c26ab1f`  
		Last Modified: Wed, 13 Oct 2021 13:28:52 GMT  
		Size: 78.5 KB (78477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90eae1289df0e0aa2e12d0696ad2612e614fc07bb39dbf50dc4a6ae357fed75c`  
		Last Modified: Wed, 13 Oct 2021 13:28:50 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aeaa98e9c1b3faaa7b199ce3ab2846597519110e0896ace6001bd3f44d2ff4`  
		Last Modified: Wed, 13 Oct 2021 13:28:50 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9966c4c9f131214a997fa36086d180d322831ea092187340ce2ad312d3db20`  
		Last Modified: Wed, 13 Oct 2021 13:29:28 GMT  
		Size: 145.1 MB (145069805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6dad85f7ab7e02bfba9b53daabfa734a2a4345b476c47bf0ed4abb6a738e00`  
		Last Modified: Wed, 13 Oct 2021 13:28:50 GMT  
		Size: 52.4 KB (52355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a302842578dbfdfa64a8e4e59ab8a088db8bbadd83aa4bfe44e944dd35687826`  
		Last Modified: Wed, 13 Oct 2021 13:28:50 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
