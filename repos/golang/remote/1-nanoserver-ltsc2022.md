## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:193292c8885322774dc03da840bff3e160dea7c48d014874537c226c04b98460
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull golang@sha256:77dedaef8da758dc4c871f21896bea0b2d7022d1da41638019abfaf30e158c7b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.8 MB (228840450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8e5416bf3db9426ac3f9d98c77fda2f8143814d0e15262844f2ca8d785ece6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 20:38:35 GMT
SHELL [cmd /S /C]
# Thu, 13 Jul 2023 20:38:36 GMT
ENV GOPATH=C:\go
# Thu, 13 Jul 2023 20:38:36 GMT
USER ContainerAdministrator
# Thu, 13 Jul 2023 20:38:50 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 13 Jul 2023 20:38:50 GMT
USER ContainerUser
# Thu, 13 Jul 2023 20:50:00 GMT
ENV GOLANG_VERSION=1.20.6
# Thu, 13 Jul 2023 20:51:50 GMT
COPY dir:25ce036b5dae3a52fa31b69c0aadfc7fed5787d8a208e86cf77a591ece610aa2 in C:\Program Files\Go 
# Thu, 13 Jul 2023 20:52:12 GMT
RUN go version
# Thu, 13 Jul 2023 20:52:12 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:cc0a26bd90fcc4d863317c36d7ffec77a0a82a905697204d4dcbc76ec13b3920`  
		Last Modified: Tue, 11 Jul 2023 20:10:45 GMT  
		Size: 120.1 MB (120056465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262f95c9ffc2400b306c39bdd21ab1ee5e02c305fa1895921355e39b04ef5049`  
		Last Modified: Thu, 13 Jul 2023 21:09:57 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d65723d6c5290f74027190acf1ee9ba18c9d51dd97ae7d43aa55180c5dcdff`  
		Last Modified: Thu, 13 Jul 2023 21:09:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ebd208492d6e9b4540041dcd87d92206bc12bdf6b234dd276ad2d81738dae`  
		Last Modified: Thu, 13 Jul 2023 21:09:57 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364d1293eec57c6600f83d614d2e6f78ac8fb57a6c20691027ca7db38dbda83f`  
		Last Modified: Thu, 13 Jul 2023 21:09:57 GMT  
		Size: 86.7 KB (86715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39c7d947e695d0076bd41e61d92b006bea76bce898a31501288817066d0b8b7`  
		Last Modified: Thu, 13 Jul 2023 21:09:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62017adf63d39f9bda382ba940d63b3abe1a5a97d8855c58ee31206e88b9249c`  
		Last Modified: Thu, 13 Jul 2023 21:12:21 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c09be7af4a805dbfba392988dba7d4ce32bdc3e531b6ccde459afdad49fba8`  
		Last Modified: Thu, 13 Jul 2023 21:12:44 GMT  
		Size: 108.6 MB (108642041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b759aba2780123975208cba6452428f9f1f43aa578b6e838265679b9a42eac4`  
		Last Modified: Thu, 13 Jul 2023 21:12:21 GMT  
		Size: 48.1 KB (48064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bb28a34e4c65737501f09c6d9a67efaeea45f36ca667c6c7960d7ae6ba6c11`  
		Last Modified: Thu, 13 Jul 2023 21:12:21 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
