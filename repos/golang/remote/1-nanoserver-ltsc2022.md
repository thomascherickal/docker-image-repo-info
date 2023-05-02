## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:85ebf8090cc14cd870f275b4f51f84013aa86585a386547bea92af5b4dbdf000
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

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
