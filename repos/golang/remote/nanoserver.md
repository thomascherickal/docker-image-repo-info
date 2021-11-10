## `golang:nanoserver`

```console
$ docker pull golang@sha256:7dfa14453deb2ffb95e80bd174f2b6cf202333f4e707567b5f1ea77cd4ceb2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `golang:nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull golang@sha256:2fb0dba31d352c84ad20500f9d0aa8f301c5c0cfb52922c95c81392212ea99b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262362198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12035665c10137e14d621762873279bd5c997a1b49db6ec3cd64e960737b06cd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 13:37:46 GMT
SHELL [cmd /S /C]
# Wed, 10 Nov 2021 13:37:46 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:37:47 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 13:38:25 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 10 Nov 2021 13:38:25 GMT
USER ContainerUser
# Wed, 10 Nov 2021 13:38:26 GMT
ENV GOLANG_VERSION=1.17.3
# Wed, 10 Nov 2021 13:40:32 GMT
COPY dir:109abd4b7de9c681888d02224b53efb3555fcce4cf01c933658c41331cc240cb in C:\Program Files\Go 
# Wed, 10 Nov 2021 13:41:25 GMT
RUN go version
# Wed, 10 Nov 2021 13:41:26 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:10d992a589a3ae9381768ac49d33610737b9d4229b1e142eb81c933bc18bab3d`  
		Last Modified: Wed, 10 Nov 2021 14:06:44 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe412e1eb92d2ce39086e8e3a6cbf14e85562659c252621eddb42083af428da`  
		Last Modified: Wed, 10 Nov 2021 14:06:44 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12b2791f99d57e11ce205d8d3e714391f1bdabe469d8c390f744462a9a13bc1`  
		Last Modified: Wed, 10 Nov 2021 14:06:44 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acf946a4ef74f9ecb59a8ba6f08956ab52a7997260d6ca02d2a753cfbe03440`  
		Last Modified: Wed, 10 Nov 2021 14:06:44 GMT  
		Size: 104.5 KB (104506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862fbd33abc7472e4616495a17e3553b5b80707464930cf8f4e27bccc4564dd9`  
		Last Modified: Wed, 10 Nov 2021 14:06:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a5be1fd73c8c3fc6b2c40f6b70cdcd384098f0433e1600435af215ba90f57d`  
		Last Modified: Wed, 10 Nov 2021 14:06:41 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e75eb659466c9b728d3318fa50dc4d069b0fdefa06bafd12d01028f402bd5d`  
		Last Modified: Wed, 10 Nov 2021 14:07:13 GMT  
		Size: 145.1 MB (145061476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c43bb51ffa7d7bcbd9ae1fc86ed80c3a374488a0e08c049487a5d8581a39b6`  
		Last Modified: Wed, 10 Nov 2021 14:06:42 GMT  
		Size: 72.2 KB (72198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ab993854b92b540d5145106881f194f7e2d65e27340fedd64a3e13372b5f8f`  
		Last Modified: Wed, 10 Nov 2021 14:06:42 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull golang@sha256:61ef2e614aca3f3eb20d7857ff8732125b94ce55dee58f8e21fd53cabd7aac69
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (247993738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2e89321ed94d8a668d52cbd9cf3a910e7480ea8340d51fded52ba207cabba1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 13:41:43 GMT
SHELL [cmd /S /C]
# Wed, 10 Nov 2021 13:41:44 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:41:45 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 13:42:07 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 10 Nov 2021 13:42:08 GMT
USER ContainerUser
# Wed, 10 Nov 2021 13:42:09 GMT
ENV GOLANG_VERSION=1.17.3
# Wed, 10 Nov 2021 13:44:11 GMT
COPY dir:109abd4b7de9c681888d02224b53efb3555fcce4cf01c933658c41331cc240cb in C:\Program Files\Go 
# Wed, 10 Nov 2021 13:44:57 GMT
RUN go version
# Wed, 10 Nov 2021 13:44:57 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9fe7a02124d29cd21b5f6d5ea22a1ba3de09099c347d1d0c0e2d89e650ddee00`  
		Last Modified: Wed, 10 Nov 2021 14:07:31 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d8752875475e46882f96ac17083c461cf7d15c710cac4c1a8cd8d33325206`  
		Last Modified: Wed, 10 Nov 2021 14:07:31 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3fa850938d1b3e4fd59b7f878fd017c726deb7aa7e036fbb3e5168c8916b7a`  
		Last Modified: Wed, 10 Nov 2021 14:07:30 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e807daf8080deabcaa2a81b1c0275d8c66f9a433b607ef7db607a70fbd55bd1`  
		Last Modified: Wed, 10 Nov 2021 14:07:30 GMT  
		Size: 67.7 KB (67722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fbe59e02252cd92e606579e15cbb16ef420c9a401f6eee4d4e117f5265a115`  
		Last Modified: Wed, 10 Nov 2021 14:07:28 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e23cfe063f3fcb1dea8db6cfa315fcbe962c7071f50f95ee2950e489762a3`  
		Last Modified: Wed, 10 Nov 2021 14:07:28 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a15ec348a93995c11d6c7aa56010714afa9bce9212e06c9b99815da8cde9f`  
		Last Modified: Wed, 10 Nov 2021 14:08:00 GMT  
		Size: 145.1 MB (145061247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf586c513fcd5768829b650af564fe3c0406095c9689024fd459da20b60e364`  
		Last Modified: Wed, 10 Nov 2021 14:07:28 GMT  
		Size: 74.7 KB (74723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c0251e19f894af098721a6e9a86f44d00a3f1bd163c6d723f35d895049536`  
		Last Modified: Wed, 10 Nov 2021 14:07:28 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
