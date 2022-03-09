## `golang:rc-nanoserver-1809`

```console
$ docker pull golang@sha256:94184684f18e13a4c7a3e7413aa3bddab8f88931c560eef788ed795329315d2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `golang:rc-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull golang@sha256:eb8d3e7c0297769e20e30a62af307e66fc0852753c5591a17087e153168055f4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255402749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:463ee5a1855375b9de9f9b98f0f473a08c9b59332d5ef12c2abd38b535862313`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 20:14:56 GMT
SHELL [cmd /S /C]
# Wed, 09 Mar 2022 13:28:42 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:28:43 GMT
USER ContainerAdministrator
# Wed, 09 Mar 2022 13:29:14 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Mar 2022 13:29:15 GMT
USER ContainerUser
# Wed, 09 Mar 2022 13:29:16 GMT
ENV GOLANG_VERSION=1.18rc1
# Wed, 09 Mar 2022 13:31:22 GMT
COPY dir:b4cdac915f93d3c62dec6b31fdb0e1c28bf8e2957d4d869a190caa72662ea4b0 in C:\Program Files\Go 
# Wed, 09 Mar 2022 13:32:04 GMT
RUN go version
# Wed, 09 Mar 2022 13:32:05 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f64bdb56c2b15796c35e920619553b18bea7fbac60e4268edd3d421d55630a01`  
		Last Modified: Tue, 08 Mar 2022 20:46:00 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb485da234231f6c6bc790bde2fac723c254138ec71b37c4c56ad4594a753bd0`  
		Last Modified: Wed, 09 Mar 2022 14:10:18 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee61cb95026b98532cb3261086dd5675ed1824b9319e31666fd3d1ada84685c7`  
		Last Modified: Wed, 09 Mar 2022 14:10:18 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19946c7ffba7bc5b5c6bfa65f290bf4e72be9e69b7f9737cd37ee085ab1834`  
		Last Modified: Wed, 09 Mar 2022 14:10:17 GMT  
		Size: 71.2 KB (71193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da14b80823ca390f9514f846c4f1e8ffc5c7fe1f6880a3e0bac73dd271d57f`  
		Last Modified: Wed, 09 Mar 2022 14:10:15 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd7b8833f66c46b3008db84a60015240ef81cece0812ef071579c352b762312`  
		Last Modified: Wed, 09 Mar 2022 14:10:15 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cbd814652f303e9488c0532c4880dcba23a7eb3eb8d3dfc8bca9ba1d1ea90`  
		Last Modified: Wed, 09 Mar 2022 14:11:03 GMT  
		Size: 152.2 MB (152226827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ee3102eafb5fc0853448d2a8693ec0e73270bb2191cd3d9e8c405769715970`  
		Last Modified: Wed, 09 Mar 2022 14:10:15 GMT  
		Size: 43.1 KB (43079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa7b4b6ec60f155812ea4165c8333f231a5eb61fdb8b35b3c94097e458aeb2`  
		Last Modified: Wed, 09 Mar 2022 14:10:15 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
