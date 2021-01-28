## `golang:rc-nanoserver`

```console
$ docker pull golang@sha256:acebc08585f3964b805e6f75e15201e547147740725b2b0f8a8746f61f71330a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `golang:rc-nanoserver` - windows version 10.0.17763.1697; amd64

```console
$ docker pull golang@sha256:969848a2675a2d2896651eedbdf0fefe389327b7d3ffd72f78c591811ab9f18c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.9 MB (242947411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6289ede699b47776377a5af2c3ed80e6fdf0af620dbd917f9903ed796cd50d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 13:44:35 GMT
SHELL [cmd /S /C]
# Wed, 13 Jan 2021 13:44:36 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:44:37 GMT
USER ContainerAdministrator
# Wed, 13 Jan 2021 13:44:52 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 13 Jan 2021 13:44:53 GMT
USER ContainerUser
# Thu, 28 Jan 2021 22:22:02 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:24:02 GMT
COPY dir:3b7e6c70d8e969add4fa1ce92bff5cee03616927ff5fa4b4bdcb7645dbc514d2 in C:\go 
# Thu, 28 Jan 2021 22:24:13 GMT
RUN go version
# Thu, 28 Jan 2021 22:24:14 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50358a323c5421695eacfec8cf19b70cfc54a72e6dc491bc2bfd4391d84dcaf9`  
		Last Modified: Wed, 13 Jan 2021 15:13:44 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b504f15f2836681dc74e6bf27d7be538fe7e6a6f53ea4bf3d8be6bb6545d8`  
		Last Modified: Wed, 13 Jan 2021 15:13:44 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6648d03a5b65f08b03a3cf89c0de5e57b386f48c5316121c697a7d4f12488`  
		Last Modified: Wed, 13 Jan 2021 15:13:43 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdc9022e2634f8a89707e4bfa55b2ff2a86865a3d7e5508effdc4abd5e92405`  
		Last Modified: Wed, 13 Jan 2021 15:13:43 GMT  
		Size: 66.3 KB (66267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3d33148024d9121b1452536b9df85f11745d7d415b1537823e481164375713`  
		Last Modified: Wed, 13 Jan 2021 15:13:38 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec80bf890c042e13f833fcd8a773ee242dc9e7f47da329fc0dc30ed929474a5`  
		Last Modified: Thu, 28 Jan 2021 22:27:24 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dacb7560d90cd8972dd782633632c4a215828bfbb1308ebdd62cc56dfa80522`  
		Last Modified: Thu, 28 Jan 2021 22:27:52 GMT  
		Size: 141.5 MB (141464571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a7dccf26be70d2073bd9b58103c731f75a76b2ac2601c7dde8ace58fbc1a9e`  
		Last Modified: Thu, 28 Jan 2021 22:27:24 GMT  
		Size: 70.6 KB (70565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888896bd887dc196213389a6dbfb6cff04127723ba098e2522c5c1859b0ba05c`  
		Last Modified: Thu, 28 Jan 2021 22:27:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
