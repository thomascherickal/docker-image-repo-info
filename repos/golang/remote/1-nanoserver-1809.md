## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:da75841e68de8f2aaadc7ce0d327392db96a40d0cbc8908c3bafda51781f6bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull golang@sha256:f9ab782549664602ed95114ad428b1aab0e2eaf33f848dc5d7291e95164560af
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215561884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfb5d1d0ed8f18b13bc0f1cb31aad0fe20590b0f2e17253e956a5396f0c5bb3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 00:23:53 GMT
SHELL [cmd /S /C]
# Wed, 12 Apr 2023 02:06:46 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 02:06:47 GMT
USER ContainerAdministrator
# Wed, 12 Apr 2023 02:07:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 12 Apr 2023 02:07:30 GMT
USER ContainerUser
# Tue, 02 May 2023 18:46:01 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 02 May 2023 18:47:46 GMT
COPY dir:522e0da3d6c3a6cfa6b16530131c440cc60a26151f29e0cb9d21de10dd15cbac in C:\Program Files\Go 
# Tue, 02 May 2023 18:48:00 GMT
RUN go version
# Tue, 02 May 2023 18:48:01 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e9c90f3a763714533d4a634f7ab3d23374e5208e2ac8bae4288243917bd972`  
		Last Modified: Wed, 12 Apr 2023 02:34:36 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35c9afe28a37cef3cb1ec56c5badcba3c2ef70ac637ff3f2b24bbad038f4e43`  
		Last Modified: Wed, 12 Apr 2023 02:34:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c67b3862f1f07ff6226e8e09c886848181f4bb7a77ea30f980e96fc1e4e066`  
		Last Modified: Wed, 12 Apr 2023 02:34:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21242415bcfc24df8c8c9e08ad9f2b969d0c18e5b42332312e319bc35d6f3cb`  
		Last Modified: Wed, 12 Apr 2023 02:34:36 GMT  
		Size: 70.4 KB (70412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d520bd5f035cedaba0c8165a45f68de0fe46708fc3539c9175e48879fe3fc0b`  
		Last Modified: Wed, 12 Apr 2023 02:34:34 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6312b31d34dfb1c1d60236e54a22a2662a9660cde5472146e140982011c17a23`  
		Last Modified: Tue, 02 May 2023 19:01:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f58785eae82b5856d6863ef852a7b229a58f5b1fa1cd2db435a0fe724f77e`  
		Last Modified: Tue, 02 May 2023 19:02:20 GMT  
		Size: 108.6 MB (108616266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adb285d6809c7dca1e45308696faa935592d6c55cb358db948a9328d29733be`  
		Last Modified: Tue, 02 May 2023 19:01:59 GMT  
		Size: 79.1 KB (79116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298927700ccc1d945903013f0ed1b3eba769d39277d069182889471a54c0811`  
		Last Modified: Tue, 02 May 2023 19:01:59 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
