## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:8398013585bcb204b2afc71fb130de9fc2e46c3aeaae6d9b1ca03ab864712c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull golang@sha256:f64249ad11676adb90219c218fbb2275dce4639d8ef30a045ada17e969270edc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252482207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586ec6ebaccb5e4bc013cb181fd68fbf6889baadef6864d0165928ea11ce1457`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Tue, 10 May 2022 22:32:24 GMT
SHELL [cmd /S /C]
# Tue, 10 May 2022 22:32:24 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:32:25 GMT
USER ContainerAdministrator
# Tue, 10 May 2022 22:32:50 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 10 May 2022 22:32:51 GMT
USER ContainerUser
# Wed, 01 Jun 2022 23:27:19 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:29:51 GMT
COPY dir:f2d0f4a9267a591c33858aceb464994502f206b1bde0c83972e6f9e2e21fe641 in C:\Program Files\Go 
# Wed, 01 Jun 2022 23:30:35 GMT
RUN go version
# Wed, 01 Jun 2022 23:30:36 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d7d4dec608f59eb9166ff96f59e4f4fcbda08a55e78d630ba39e558b23b3e475`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4735e17fcd180a1d905a22c771ac994a1a249e57bfdde77ef41ccf51a0e29a3`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833e97847abafba5e024c2c960a8b406785b7f11a1a3dd574f40993a068c19e4`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd374e2694dcb43adcc3181c4f72a6fd7b1432b49478e67616949e2efe9aafd`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 68.8 KB (68805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d279dc1f42008981f8d43d3f502139a3b21c0f5ca5d86ac0b9862c424b4477e`  
		Last Modified: Tue, 10 May 2022 22:59:33 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544088d8ac402da890dab3a50f88ce8b0a328aa42759853cf624e81a5b5646e2`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37f6550d5326b4b8a6a4a872523bcde4352329a121d68322d9223e78872eab9`  
		Last Modified: Wed, 01 Jun 2022 23:53:20 GMT  
		Size: 149.2 MB (149200327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c95efe5638c689acdc995c4001a617628f0f5e3879b5bc6c0146e8595afa3c`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 72.1 KB (72067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f64c487fbd419b6c977df6cbbc92087927217a8803e8535130b1745df3f0d1`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
