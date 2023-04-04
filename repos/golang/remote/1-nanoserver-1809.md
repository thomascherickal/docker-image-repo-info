## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:b8a89241dce051cddfdf9ba55df24b9288b1156fc24fc00ee90ddc73d01ab7ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull golang@sha256:0b1cbd9cc524f685c84e6923637ce5895dd0edf7460ad4fe88b51035223349d6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215443994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85195c821fe4ee51e48795f5bcafc7cebf338e0b807376d1b9d65573b35324d3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 02:20:46 GMT
SHELL [cmd /S /C]
# Thu, 16 Mar 2023 02:20:47 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:20:48 GMT
USER ContainerAdministrator
# Thu, 16 Mar 2023 02:21:31 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 16 Mar 2023 02:21:32 GMT
USER ContainerUser
# Tue, 04 Apr 2023 18:36:53 GMT
ENV GOLANG_VERSION=1.20.3
# Tue, 04 Apr 2023 18:39:29 GMT
COPY dir:7f53f5369bd810a38f3697430c98fd1ef31e62b6dbcf30f7fe02d334a38965f8 in C:\Program Files\Go 
# Tue, 04 Apr 2023 18:40:11 GMT
RUN go version
# Tue, 04 Apr 2023 18:40:12 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5cc414fce78380e134ec2315d713a8a9040bff5d1298887a2a68029cfc0922`  
		Last Modified: Thu, 16 Mar 2023 02:48:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77358ace842a4af47a00594821c3cc0c53ef0f00f3695692c2f19b6f9fd023bd`  
		Last Modified: Thu, 16 Mar 2023 02:48:05 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633faaff1da959771878c043ba820b0e38b62cf26268b1e87acd834496c3de90`  
		Last Modified: Thu, 16 Mar 2023 02:48:05 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d52a594f074a3f99c586be0721850cc97d40228451e2e289e99145906f8566`  
		Last Modified: Thu, 16 Mar 2023 02:48:05 GMT  
		Size: 69.5 KB (69550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027c3baf1644b032096e95101de22f26e2b8e43c242cac344351be66be56757a`  
		Last Modified: Thu, 16 Mar 2023 02:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f884517be37c7b33797e6c5c67e996572eadea42d424e879fdf4aca6ed3bcad7`  
		Last Modified: Tue, 04 Apr 2023 19:01:18 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6721e328886bb258dcca09328af3cea28cb1ad040f6cf82e3bcedc52049e5d1`  
		Last Modified: Tue, 04 Apr 2023 19:01:52 GMT  
		Size: 108.6 MB (108611019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9ee1e72032f9da577d50e91df44d19db9187f7656d749ab482e36069ecef53`  
		Last Modified: Tue, 04 Apr 2023 19:01:18 GMT  
		Size: 72.0 KB (72050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba321ad8e72cf141e625cab469005342d4567035e3f12faa46a1407e3c7b0a4`  
		Last Modified: Tue, 04 Apr 2023 19:01:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
