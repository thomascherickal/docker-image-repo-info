## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:3d43a7421ccee4d81a1f94167d578b0d6b2e50d60baeea6e8e38739c03b60a07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull golang@sha256:85ac8d22d6ca56d10d05ae85a57018ff1a901c3ec6f8c6cf2986650ccc08ce5e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230196729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0d5a3efbffaa4fd1725a5caf76a0c2f8af117f2f7c1b9acc01e91f2776aac9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 06 Jan 2023 23:36:49 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 03:07:34 GMT
SHELL [cmd /S /C]
# Thu, 12 Jan 2023 03:07:34 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:07:36 GMT
USER ContainerAdministrator
# Thu, 12 Jan 2023 03:08:26 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 12 Jan 2023 03:08:27 GMT
USER ContainerUser
# Tue, 14 Feb 2023 20:23:26 GMT
ENV GOLANG_VERSION=1.20.1
# Tue, 14 Feb 2023 20:26:11 GMT
COPY dir:e8adf0c358ef6b81c93fbb960ba193f8e4b0591afd1ed47065f1c9b7dcb3528e in C:\Program Files\Go 
# Tue, 14 Feb 2023 20:27:09 GMT
RUN go version
# Tue, 14 Feb 2023 20:27:10 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:83e9437e818022c1c28f0e07002dd46995c8614e62b9366138fa23b94f43d9ad`  
		Last Modified: Thu, 12 Jan 2023 02:51:06 GMT  
		Size: 122.1 MB (122099566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e0e139d1c09b743fda52fd8a19bdc3c829ac2aed829d2e16beec0fbbd5dd5d`  
		Last Modified: Thu, 12 Jan 2023 03:48:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e8737aebbf1207ce8659de66f3d575194350678800b69a174bc516a329dea`  
		Last Modified: Thu, 12 Jan 2023 03:48:59 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611ab0a2da8d60a13ec497aa6f89b840f936a6c6f7450f0386f808c000f44970`  
		Last Modified: Thu, 12 Jan 2023 03:48:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c63725f8ca8d354e6c46948328eda4a7c428e21bfedbd5005b674e23fbf73`  
		Last Modified: Thu, 12 Jan 2023 03:48:59 GMT  
		Size: 84.0 KB (84048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b910fe2ecce44f108e85c2c03f9acb106e857aa6b7f2e4622891aa961b4bf`  
		Last Modified: Thu, 12 Jan 2023 03:48:57 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03bd53e831b6365e1bb9cfb508f31d2bbe56e21264d553d9fe11ad082c1d43f`  
		Last Modified: Tue, 14 Feb 2023 20:53:15 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9ba94dc3bd307a34d8b68b3befb35230fafee34edf15c95d82ab4d25f8dd1c`  
		Last Modified: Tue, 14 Feb 2023 20:53:52 GMT  
		Size: 108.0 MB (107956055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14582034cf087b622be10471e490fedc7b8c81e58e8ef43bd94d2fc59c7a0ac7`  
		Last Modified: Tue, 14 Feb 2023 20:53:15 GMT  
		Size: 50.1 KB (50103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684d95104ae1d4954b6909061b675796d966226d487d4f2eb0fc6d9216dba164`  
		Last Modified: Tue, 14 Feb 2023 20:53:15 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
