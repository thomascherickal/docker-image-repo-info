## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:710af9ca3c9e5822b82d09e6a454b28c2df7f38d2362740a8b10ed5a79073208
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull golang@sha256:d06cb291c3c2ace8dbc0e3ac665f3fb3e435079b786c25f5319ee5c53cfde08f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252475392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fc87a725bd7570a5e61b3e3d6d5d41fc24dfd8b6091c2de090482f8f03063e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Tue, 12 Jul 2022 19:43:41 GMT
SHELL [cmd /S /C]
# Tue, 12 Jul 2022 19:43:42 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:43:43 GMT
USER ContainerAdministrator
# Tue, 12 Jul 2022 19:44:22 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 12 Jul 2022 19:44:23 GMT
USER ContainerUser
# Tue, 12 Jul 2022 20:00:32 GMT
ENV GOLANG_VERSION=1.18.3
# Tue, 12 Jul 2022 20:02:54 GMT
COPY dir:f2d0f4a9267a591c33858aceb464994502f206b1bde0c83972e6f9e2e21fe641 in C:\Program Files\Go 
# Tue, 12 Jul 2022 20:03:41 GMT
RUN go version
# Tue, 12 Jul 2022 20:03:42 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c14e0078b75f39dd734aa5bda1a20ee6aea0391d04d7986262fa35b4ee1b4046`  
		Last Modified: Tue, 12 Jul 2022 20:24:02 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58123f14ee126159f65688fa93c48fd79e7accdb32597dd01733e08a7f53dc2f`  
		Last Modified: Tue, 12 Jul 2022 20:24:01 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fc8029652a8954a5a99d5f3a33f6fdb9063693255e805a20b8963c195815fb`  
		Last Modified: Tue, 12 Jul 2022 20:24:01 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3769b7ac07e824a5ed356258fa6870ca8df0bd37ab1cf016a3033d9a2943f6c1`  
		Last Modified: Tue, 12 Jul 2022 20:24:01 GMT  
		Size: 69.4 KB (69434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dabb95e3ef99b306d606ea8969c68055e25dcada3a0f64ead470fd2f7729835`  
		Last Modified: Tue, 12 Jul 2022 20:23:59 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5665e7e196bbbd6ba3dbdfc0c7285454f16f27a161702562f43d51bd2c08c8e`  
		Last Modified: Tue, 12 Jul 2022 20:28:30 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e7124159c8f0315cdb25a335355c71c0a4f62823460c612698dd3359961928`  
		Last Modified: Tue, 12 Jul 2022 20:29:19 GMT  
		Size: 149.2 MB (149172683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506e42efb8d098aa9646c3532859f4287c6d91f1711e1228659eb82b6c96f88`  
		Last Modified: Tue, 12 Jul 2022 20:28:31 GMT  
		Size: 71.3 KB (71320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aec45cc8d6156c59a68042da2bdd131dc4495f4ca1ce512f1f2515a361585d3`  
		Last Modified: Tue, 12 Jul 2022 20:28:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
