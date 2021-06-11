## `golang:rc-nanoserver`

```console
$ docker pull golang@sha256:3a5d95125718b9e6d7bf505afd9754cb3f6268144a330a2d0aa75181d07ca625
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `golang:rc-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull golang@sha256:05d78ae7b6bac7e62ee14f9b229b2eda6f94722d2568aa6b10b76e809bcc0436
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.6 MB (247563706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1adffb08ae756b169e897dc949a97252c0533c688b70a81f8f01607db9d0858`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 12:49:37 GMT
SHELL [cmd /S /C]
# Wed, 09 Jun 2021 12:49:40 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:49:43 GMT
USER ContainerAdministrator
# Wed, 09 Jun 2021 12:50:14 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 09 Jun 2021 12:50:17 GMT
USER ContainerUser
# Thu, 10 Jun 2021 21:23:57 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 10 Jun 2021 21:26:18 GMT
COPY dir:b6d7964daa3a40e803fca5841706cb4fae8b0243268db925ad07755564d68668 in C:\go 
# Thu, 10 Jun 2021 21:26:48 GMT
RUN go version
# Thu, 10 Jun 2021 21:26:50 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2646c4431bb01c2667bc3bd1353d18b2632d04cc58ad53a79480ecdde4fd710d`  
		Last Modified: Wed, 09 Jun 2021 13:05:18 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb2068fe4d0d7f614dcebdadd3eb0af27aa70abda1ebb8dee1bfd37c791197a`  
		Last Modified: Wed, 09 Jun 2021 13:05:17 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8563765367d01f674014a0e8ad51aee3b3cf8967835b6f641d121994ccd72fb9`  
		Last Modified: Wed, 09 Jun 2021 13:05:18 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e027a5dbd9c579ecc14f1a4e5987be4fd5b701b2a4518041acd65713b2a3eb24`  
		Last Modified: Wed, 09 Jun 2021 13:05:17 GMT  
		Size: 68.6 KB (68632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6609d2c783fad47fae875fcad47c9339cb27ee403677d7de00729023bc437d`  
		Last Modified: Wed, 09 Jun 2021 13:05:15 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474a50ba355a7de9ac46ecbd351d3974ba7145f09d616033533ad5c9c519b59f`  
		Last Modified: Thu, 10 Jun 2021 21:34:37 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46e015b159a62df4ba02853eb670be7297ff42e53124531351c7b9051bb1207`  
		Last Modified: Thu, 10 Jun 2021 21:37:26 GMT  
		Size: 144.7 MB (144745789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8606d37c12a5030a1c7a8231d81ea20c5449ac8f4ee6ea2aee50c605e1297`  
		Last Modified: Thu, 10 Jun 2021 21:34:36 GMT  
		Size: 70.7 KB (70715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2398113e25b01ef2e01f7537e767c7524c0c24c941c2d0c1e57c00e3d481e`  
		Last Modified: Thu, 10 Jun 2021 21:34:36 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
