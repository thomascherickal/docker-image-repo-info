## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:b628a3ed1a3aad52ee5feb6c525fa461091d79183eca8a5ec2282b7727908ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull golang@sha256:86283f3216defd950ac19cd237f42fae73321c6b7b9d7eac9934a4747c6cd52f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234131308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fed26c551aaac102ea1af3570266729903b756fe955e01080463c3b733a55c5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 12:22:44 GMT
SHELL [cmd /S /C]
# Wed, 11 Mar 2020 12:22:45 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Mar 2020 12:22:46 GMT
USER ContainerAdministrator
# Wed, 11 Mar 2020 12:23:03 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 11 Mar 2020 12:23:04 GMT
USER ContainerUser
# Thu, 19 Mar 2020 23:22:25 GMT
ENV GOLANG_VERSION=1.14.1
# Thu, 19 Mar 2020 23:24:40 GMT
COPY dir:570ee6417f99b886b2997b09f722ea0416d1c6c9c053b0e5f0ef8f9678c726ae in C:\go 
# Thu, 19 Mar 2020 23:24:59 GMT
RUN go version
# Thu, 19 Mar 2020 23:25:00 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5bd48aea83b7e2963ae4ac0db2f96681643b4dc342cb3946ca3e871118d13dc`  
		Last Modified: Wed, 11 Mar 2020 12:44:25 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5477696fd9e22926db0f7309a634f6944f820196822afefa1ac999b75c02547`  
		Last Modified: Wed, 11 Mar 2020 12:44:25 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59b57411eae55dbcd4b8866c459b097d96859ab5b362bf55915c63a137cab1`  
		Last Modified: Wed, 11 Mar 2020 12:44:26 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4945c92290e8b2226499045f6b2ae5ca967c87c1b8f99eb649a1ae4f6fa1ec`  
		Last Modified: Wed, 11 Mar 2020 12:44:25 GMT  
		Size: 63.6 KB (63586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd405078311545e65484faccb35564c272103e6b9e1d0323f9e76f718cf6188`  
		Last Modified: Wed, 11 Mar 2020 12:44:22 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56d51b34ef64d5a6012ade740f2cc7020f991a6d11f75c2071e033673e3b632`  
		Last Modified: Thu, 19 Mar 2020 23:36:47 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f486211a903e353af9eb5fecf806f1a65caf25d80fdb673bc364ba308f4aeb0c`  
		Last Modified: Thu, 19 Mar 2020 23:37:14 GMT  
		Size: 132.9 MB (132941488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0815708678a4f7e5d22b68e6791ed558921a5552d7bb42d8ced75e6315da4d`  
		Last Modified: Thu, 19 Mar 2020 23:36:47 GMT  
		Size: 70.1 KB (70125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eed014b79ed984732b5d3fcad22bda800e2d74f228ba6efd2a1ee9db71d876`  
		Last Modified: Thu, 19 Mar 2020 23:36:47 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
