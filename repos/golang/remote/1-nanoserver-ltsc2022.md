## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:73d0a18c8416f785797ef229a8af066cd0bd4fc03f7b06398f8748a826c098cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull golang@sha256:d08dfe442c8d0dbd180c883198dbcf881e47f8a48ecd301c2d015b64c665da69
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189566083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067cc8a98157422db7fd1c72816c0f07b1b1f51c08d241d120a96312e229184e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Aug 2023 09:40:19 GMT
RUN Apply image 10.0.20348.1906
# Thu, 10 Aug 2023 00:45:25 GMT
SHELL [cmd /S /C]
# Thu, 10 Aug 2023 00:45:25 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:45:26 GMT
USER ContainerAdministrator
# Thu, 10 Aug 2023 00:45:41 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 10 Aug 2023 00:45:42 GMT
USER ContainerUser
# Thu, 10 Aug 2023 00:45:43 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:47:36 GMT
COPY dir:c21970be5995b3ef4606ef40facc4d16ec9885a3650e5902951dfb757ebb0503 in C:\Program Files\Go 
# Thu, 10 Aug 2023 00:47:59 GMT
RUN go version
# Thu, 10 Aug 2023 00:48:00 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:ea9613880997b3ab2284a37c0c14a403553457b0c331b41c6bd6d1cc7838a222`  
		Last Modified: Tue, 08 Aug 2023 18:47:21 GMT  
		Size: 120.5 MB (120500677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a528e77cf0bef98e15c3b4194ee340960485498ac4c1bdcbab44307858ecfc4`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4287adcc177140a1d49ede9aba58d0e4266daff7899156f821c228ff5e26e4`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165623060fccc8fd72ac1aee74f9dec194514da3ad631a694c4dadd39a7efc93`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41934ff5e4a1f7de6165371bf05245eba59f79a718a0e4c63b0c1272984e97a`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 77.2 KB (77192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766ddc6fd21c9745584f53d5f3ae272f830b0f0fed2455fc7c84ce55600a2b0`  
		Last Modified: Thu, 10 Aug 2023 01:03:24 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2fa7497b7abafbc86252e86560d3684dd83d4257f0f1a75ad807ebd22440be`  
		Last Modified: Thu, 10 Aug 2023 01:03:24 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ed67c62d481a40a979079b5521be9e2b38b28543166b026e4b65add4e1f99d`  
		Last Modified: Thu, 10 Aug 2023 01:03:43 GMT  
		Size: 68.9 MB (68928557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4f7a99f7f0fdc78667e3a4bce874ed36fa4816acc82af03a728fc941d9526d`  
		Last Modified: Thu, 10 Aug 2023 01:03:24 GMT  
		Size: 52.6 KB (52555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c475eef924f269d3d72701b47281a0c3c36dc4740bffc22805043161b3f1c10`  
		Last Modified: Thu, 10 Aug 2023 01:03:24 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
