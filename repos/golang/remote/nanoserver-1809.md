## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:c77dc208ff83d4cf14b8d08284940d76314bbe918dd527a9625ce9abafe3fffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull golang@sha256:23547034e3c6778035998dabfc451d232e4a75efe5f02629c08225fd5746ab19
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234205761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9db2c29bb45feba2d33d1b4b56f4d2fa4f74d2d08879c5c2b46ed3c70da896`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 12:24:27 GMT
SHELL [cmd /S /C]
# Wed, 10 Jun 2020 12:24:27 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Jun 2020 12:24:28 GMT
USER ContainerAdministrator
# Wed, 10 Jun 2020 12:24:44 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 10 Jun 2020 12:24:44 GMT
USER ContainerUser
# Wed, 10 Jun 2020 12:24:45 GMT
ENV GOLANG_VERSION=1.14.4
# Wed, 10 Jun 2020 12:27:10 GMT
COPY dir:79141300d8757e9df6bce16180e905d9ccf2155e9a1263e19d03686a5c1d4794 in C:\go 
# Wed, 10 Jun 2020 12:27:25 GMT
RUN go version
# Wed, 10 Jun 2020 12:27:26 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ccc2ab174115d7c1f51c57b207bdadd2668d5de4d6f81a62f1dc59b31df7f15b`  
		Last Modified: Wed, 10 Jun 2020 12:39:48 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9583d464994f7875d7c8cb87eed53cca0febfb7858a842e2c50062e033fac949`  
		Last Modified: Wed, 10 Jun 2020 12:39:48 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b915241332cbe27b35f3eb233a8c2d632493880ddc7a5ab772d4fc00a32cdf`  
		Last Modified: Wed, 10 Jun 2020 12:39:47 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1088d70f6361299e2ed3757ecf7c4b4194b7086ba6bb0657ec5846d430669097`  
		Last Modified: Wed, 10 Jun 2020 12:39:47 GMT  
		Size: 67.4 KB (67379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056ad564aad66a81fc80e987921a29f646707699d3ad7cb8e074426e0015d24`  
		Last Modified: Wed, 10 Jun 2020 12:39:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e11da173f991f537c96b980972902c6f926329829ef959d3fe68e9cf7a829`  
		Last Modified: Wed, 10 Jun 2020 12:39:45 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9557c31afe7cba9ef36a897188cdc7bd0277eb043ccab8e466e59b3d40acf899`  
		Last Modified: Wed, 10 Jun 2020 12:40:11 GMT  
		Size: 133.0 MB (133016653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a70d23f83b90cbb169add4668503c6eb0c5aa5907d63c012d119a7da33aaa1`  
		Last Modified: Wed, 10 Jun 2020 12:39:45 GMT  
		Size: 72.8 KB (72834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010db5e1432bbc6c8a4abc77e0a70358bb5df052b8413b1a2471adcbd6a47f3f`  
		Last Modified: Wed, 10 Jun 2020 12:39:45 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
