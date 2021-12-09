## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:3fd93909070c9ac534eb3a08c6990ab0f100802a8c0521beac56ba82ccfb1b81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `golang:1-nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull golang@sha256:fc3992340f2339aaa528268d30de2c8ac043cb58faceaa5df0129643dce0f2c8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262371669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e3078a4b984c5728e3a9cab9a2bb00c5f9ee85efe2ff8005c65830dbd669c2`
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
# Thu, 09 Dec 2021 16:27:10 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:29:31 GMT
COPY dir:4c99dbbc4d53a915cdc29ae9417d812da5b5217c7296fe04ef7fdf708c4a960d in C:\Program Files\Go 
# Thu, 09 Dec 2021 16:30:24 GMT
RUN go version
# Thu, 09 Dec 2021 16:30:25 GMT
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
	-	`sha256:227be6d567676f0cbdcb9b197b5baef7cb0e5c9092b6df1bd2f55d520954827e`  
		Last Modified: Thu, 09 Dec 2021 16:54:58 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf5f3c0f0561d52669b18aa0e5b9668f4bdab9c0687ae346b1b4f8c5acb0ba6`  
		Last Modified: Thu, 09 Dec 2021 16:55:32 GMT  
		Size: 145.1 MB (145073825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0e7bd126e3bab5dda952db7989d17cac3c780cdb4876239d5807632d207d0a`  
		Last Modified: Thu, 09 Dec 2021 16:54:59 GMT  
		Size: 69.4 KB (69410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37edcde80e9d8e32bad22d06571f478dcb79270d91071df53ad623257e2e681`  
		Last Modified: Thu, 09 Dec 2021 16:54:58 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull golang@sha256:921d5a9f3f2aae5181394f148cbfd73564e891c637cbcb6101e6012a68000a22
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (248007761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36226b7d734716b73f62d12180958466b68f2500f84bad6c8a8395b1914e6d93`
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
# Thu, 09 Dec 2021 16:30:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:32:54 GMT
COPY dir:4c99dbbc4d53a915cdc29ae9417d812da5b5217c7296fe04ef7fdf708c4a960d in C:\Program Files\Go 
# Thu, 09 Dec 2021 16:33:41 GMT
RUN go version
# Thu, 09 Dec 2021 16:33:42 GMT
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
	-	`sha256:b54b5f3d654dad2968536c381119dd5c5eeee23177ae791e175c4dcd56bfea1e`  
		Last Modified: Thu, 09 Dec 2021 16:55:47 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56d9e375a5b49fe0b3df01e177940fa42c7bc636b5ce543ed506b48249976da`  
		Last Modified: Thu, 09 Dec 2021 16:56:21 GMT  
		Size: 145.1 MB (145078303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ccadab925ee644daa59f062459bc8003a43bd4de5ca30a3f1d170ee7a06550`  
		Last Modified: Thu, 09 Dec 2021 16:55:47 GMT  
		Size: 71.6 KB (71639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3805c72011c0e4301cf66491c38b7187d540115f213240b523446b093aeef5`  
		Last Modified: Thu, 09 Dec 2021 16:55:47 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
