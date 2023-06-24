## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:a590e541477e2e0adc6c5a878ebffbdf9517a8615522207eab81e5205782350f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull golang@sha256:b59b243dc39e1850b741ad62ed468eca0b78c3479b4b95876277028c12548ef0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.8 MB (228788590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a0990b561f4c0a277a0f33aff73a48c4d9462bb178bd8acb307854125df174`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:47:25 GMT
SHELL [cmd /S /C]
# Sat, 24 Jun 2023 01:47:26 GMT
ENV GOPATH=C:\go
# Sat, 24 Jun 2023 01:47:27 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:47:50 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Sat, 24 Jun 2023 01:47:51 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:58:36 GMT
ENV GOLANG_VERSION=1.20.5
# Sat, 24 Jun 2023 02:00:27 GMT
COPY dir:2b56775b246889ea39ed6a295f7604dfecd0a015e0fc1352d091198ccc0b1678 in C:\Program Files\Go 
# Sat, 24 Jun 2023 02:00:45 GMT
RUN go version
# Sat, 24 Jun 2023 02:00:46 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b2deb8649e4dedd9fbe74195175cfdae8176065d0daa61337779d26f0bce93`  
		Last Modified: Sat, 24 Jun 2023 02:17:36 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9e10cc3f3d5c676eb7a8f8b4ed7fe56afe4cf0350369685fa91aa510083aac`  
		Last Modified: Sat, 24 Jun 2023 02:17:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33b58becc93557f6a89d8222cf063545afd5a26b68db2507913d2c21195a0b3`  
		Last Modified: Sat, 24 Jun 2023 02:17:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc923d8d9d8150c33f7f6b2a2e36a2f4d74b75729b25a0b8e212b9c4c30b7e01`  
		Last Modified: Sat, 24 Jun 2023 02:17:36 GMT  
		Size: 85.8 KB (85779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856c8830a4f06b847fc16b25317f8f7b56b03fb5ccac5d82a17c420b2e5e7385`  
		Last Modified: Sat, 24 Jun 2023 02:17:32 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7beecf43bb34cacdfb1c1ddb2bea23b297864dd087142e9c9c7bc33b27d742f`  
		Last Modified: Sat, 24 Jun 2023 02:19:44 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa63e407c0bad92de89e7e9508c41e2f638b69fdc841b94a23e7f24ffb6630`  
		Last Modified: Sat, 24 Jun 2023 02:20:05 GMT  
		Size: 108.6 MB (108619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f9a16edd7e128e3385e596b594c901de1eaeedd2eb83e21ceb502b476add44`  
		Last Modified: Sat, 24 Jun 2023 02:19:44 GMT  
		Size: 48.1 KB (48114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b7c2a43c3540448b51a628f6ea80ae5970924684170b8c5404bb9927c0183`  
		Last Modified: Sat, 24 Jun 2023 02:19:44 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
