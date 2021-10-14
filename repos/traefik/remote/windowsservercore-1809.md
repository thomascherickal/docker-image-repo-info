## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:1958e0667a0daf324ed1594824617417ceb9177015a1a39085a1dedbd253979d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull traefik@sha256:189b71f8da5a9dac8231d86f0ae129061b5d0daae2d0011a81d1183ba022c077
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712506883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fa1da2e69cdf4c5e27af93e5a66a007a11aa8b99db703254a3cc36b3526ab4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 02:47:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.3/traefik_v2.5.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 14 Oct 2021 02:47:01 GMT
EXPOSE 80
# Thu, 14 Oct 2021 02:47:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Oct 2021 02:47:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffd862beb07529675bc9efa18496f64d0002e4f5c21080befa8ce4491fe538`  
		Last Modified: Thu, 14 Oct 2021 02:49:21 GMT  
		Size: 26.2 MB (26182410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63beef12cf0726a083eacdceec11278378e64e4cef47e4063e2b712cb410b36`  
		Last Modified: Thu, 14 Oct 2021 02:49:11 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d21a1a0c93b6bb9d13428118de996b57ea7d825a2bcb00491c44f836bc305b1`  
		Last Modified: Thu, 14 Oct 2021 02:49:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a317c1bc07eab8967b34a81e7d0b4112fd0ddfcb044d022fc29f489c9d3a71f2`  
		Last Modified: Thu, 14 Oct 2021 02:49:11 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
