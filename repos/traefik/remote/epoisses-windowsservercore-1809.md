## `traefik:epoisses-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8583fe4971cb2573a1498d586c2c406c82952b1caba30300fc43d584e06f071f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `traefik:epoisses-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull traefik@sha256:6d2b8c67d9d22624d657ef2aa8f707680353d3f353ac5d3c9c0dc03e9a2c2735
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743914830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baff7681684f92c6785dc81825222cac9978ae4a5ee8da9eca2db6c468d51a3d`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 19:00:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.0-rc2/traefik_v2.7.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Apr 2022 19:00:57 GMT
EXPOSE 80
# Wed, 13 Apr 2022 19:00:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Apr 2022 19:00:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87593a35b0484effb7c0c1555805726755eb725e89659d0048ba2577537e6736`  
		Last Modified: Wed, 13 Apr 2022 19:04:31 GMT  
		Size: 28.0 MB (27989102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255d18cf96bf0293e78bcddf95a6d48ce7ea7428dec11fcfcbeaf0f98442ac25`  
		Last Modified: Wed, 13 Apr 2022 19:04:01 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f265c059da21fe7d429f7a0762404c6c3bb27cf533697c58426adea71f0904`  
		Last Modified: Wed, 13 Apr 2022 19:04:01 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5fa4fed7fd6b0a99c476edc1561afa4c1ab826c91570f56b8809cf49b8b4b9`  
		Last Modified: Wed, 13 Apr 2022 19:04:01 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
