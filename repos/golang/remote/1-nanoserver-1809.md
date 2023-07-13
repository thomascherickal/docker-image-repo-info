## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:d4aa8b78a5174295517c01eb6ab48b759e4a2526d06edefa559642b87fe482c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull golang@sha256:edbd3913ac74ca502062c66dbdccf8c54a4bdab447b3bd6517d81c5a207fa6ab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.2 MB (213216727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f969cf227899c2839d9c6da22a389bae7fd31bf7b983de72a4d76e57fa943109`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 20:41:18 GMT
SHELL [cmd /S /C]
# Thu, 13 Jul 2023 20:41:19 GMT
ENV GOPATH=C:\go
# Thu, 13 Jul 2023 20:41:20 GMT
USER ContainerAdministrator
# Thu, 13 Jul 2023 20:41:31 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 13 Jul 2023 20:41:31 GMT
USER ContainerUser
# Thu, 13 Jul 2023 20:52:30 GMT
ENV GOLANG_VERSION=1.20.6
# Thu, 13 Jul 2023 20:54:20 GMT
COPY dir:25ce036b5dae3a52fa31b69c0aadfc7fed5787d8a208e86cf77a591ece610aa2 in C:\Program Files\Go 
# Thu, 13 Jul 2023 20:54:38 GMT
RUN go version
# Thu, 13 Jul 2023 20:54:39 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48271163dd58fddb2ff623ae3c53cac64a29148ad84e995c93073602f68793d`  
		Last Modified: Thu, 13 Jul 2023 21:10:35 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8c1feea8292b9bc0b0f2be869e9692d63d21efa75624c84fa878079e30b05`  
		Last Modified: Thu, 13 Jul 2023 21:10:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8041e971a244f1bdd7e444ce782b9e6fa4ba5859f2bbc2b8ccac016697970d7d`  
		Last Modified: Thu, 13 Jul 2023 21:10:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64db53aeff99ec4a41edd8036064f37150123d7caf2d1eff287f9704a010c6c`  
		Last Modified: Thu, 13 Jul 2023 21:10:34 GMT  
		Size: 76.3 KB (76262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25cfa96b658400676137a25a21f4628df693a06c1d217748e7696d9570cae7`  
		Last Modified: Thu, 13 Jul 2023 21:10:32 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1d379938478df76e3f1871b8a39f0e30d89b869b02b7fd702dd61cd497f3e`  
		Last Modified: Thu, 13 Jul 2023 21:13:00 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f397154992c6b66dca7b2f11d3b76db628f2b7a834ddf8e734af4998a333d33`  
		Last Modified: Thu, 13 Jul 2023 21:13:22 GMT  
		Size: 108.6 MB (108643076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888d225c54a865463eb9ba459e1d92eea4975cd46ae8fac5c161cbe8b6111c0`  
		Last Modified: Thu, 13 Jul 2023 21:13:00 GMT  
		Size: 82.1 KB (82129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576cd1515f570ed1d614799e73fe9df58c91a30a258ca16aba430ce25177d7d0`  
		Last Modified: Thu, 13 Jul 2023 21:13:00 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
