## `golang:nanoserver`

```console
$ docker pull golang@sha256:ed16a065b41c4856562f03ce1d9892782bcc43b8f8ee5efbf33f79aaa1fce82d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1668; amd64
	-	windows version 10.0.17763.4252; amd64

### `golang:nanoserver` - windows version 10.0.20348.1668; amd64

```console
$ docker pull golang@sha256:a8a16a29c11c6d25cd3fa9281a4358d7ea48d3e687d8f9503504653864ef1bba
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231104866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa28459040c5bb7f2e30007863d7b56d141ae7a848a6e841c9e0ffda657764b7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 00:22:09 GMT
SHELL [cmd /S /C]
# Wed, 12 Apr 2023 02:01:45 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 02:01:46 GMT
USER ContainerAdministrator
# Wed, 12 Apr 2023 02:02:37 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 12 Apr 2023 02:02:38 GMT
USER ContainerUser
# Tue, 02 May 2023 18:43:34 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 02 May 2023 18:45:18 GMT
COPY dir:522e0da3d6c3a6cfa6b16530131c440cc60a26151f29e0cb9d21de10dd15cbac in C:\Program Files\Go 
# Tue, 02 May 2023 18:45:41 GMT
RUN go version
# Tue, 02 May 2023 18:45:43 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329579f5fc95fa89293545a20f4e45221db45261002e7012b86c4d3233edd1f8`  
		Last Modified: Wed, 12 Apr 2023 02:33:39 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785015715e7f6f5df91d88dc81eb9ed7bc36ef9cfefd565bbf522dff9d2d481`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11e8fa20dea6ccdcfb21ddbbdb24441556806bcffdb534698b12f27ccf7a4e`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c53d49ef28647b964bc9d5a90c2567c0a8e57189eaf101b2d26cecf98953de2`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 83.7 KB (83741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed452e8d633078d3cbc8aa29b71cdb34650769d2a1b2c008738aafc6f4aed361`  
		Last Modified: Wed, 12 Apr 2023 02:33:37 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7031ba04a0fa65c75dcf69900a4e29b3e9293d5ceb5cbec1a8e0b293429ec8db`  
		Last Modified: Tue, 02 May 2023 19:01:25 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584dc0c1c837aecbf6b6f87a93ec0b046ade078d7fe1f31db2e923ca7113a35a`  
		Last Modified: Tue, 02 May 2023 19:01:46 GMT  
		Size: 108.6 MB (108633381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af87b5e03cda152ce267879c0f746de0bf427ed613bed2dea2cf6228711fedf0`  
		Last Modified: Tue, 02 May 2023 19:01:25 GMT  
		Size: 51.8 KB (51801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d691facae651310a975ebc6ed138fae9b1278170b20bd9206bb7353de3f28a`  
		Last Modified: Tue, 02 May 2023 19:01:25 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:nanoserver` - windows version 10.0.17763.4252; amd64

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
