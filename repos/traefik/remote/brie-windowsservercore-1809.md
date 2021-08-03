## `traefik:brie-windowsservercore-1809`

```console
$ docker pull traefik@sha256:aef3f0b0c609e375cec9b2d66ae9d75e8c589b671bd329800ceadf3c118ed306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `traefik:brie-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull traefik@sha256:e563ab27a269f011ee98bdcd8a0305e8ad8d1070597a96d4f7e986e70274a10c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712518943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61094862b1046697bab586abb532d5d4c2ddeae35b750ca7fbfbb77c7c09ce41`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 03 Aug 2021 20:26:48 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.0-rc5/traefik_v2.5.0-rc5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 03 Aug 2021 20:26:51 GMT
EXPOSE 80
# Tue, 03 Aug 2021 20:26:53 GMT
ENTRYPOINT ["/traefik"]
# Tue, 03 Aug 2021 20:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0-rc5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8a767328a80a21ac17180baa21c4c24f44b7d62e9033f0a03b56c5ebb832f4`  
		Last Modified: Tue, 03 Aug 2021 20:27:42 GMT  
		Size: 27.1 MB (27066452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbf0181956e176cfee9493349f4d35cface59da6a54b66f2fed8110fd70df3`  
		Last Modified: Tue, 03 Aug 2021 20:27:35 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b650a1e6c11998c300f7ec12e953e6fe98ee972bcf58cb1ec04aab263e16d5`  
		Last Modified: Tue, 03 Aug 2021 20:27:35 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e7b1399fe2a6af7f2ff7b759abe6e78203efa10eaab4e6cd367cb047af4b30`  
		Last Modified: Tue, 03 Aug 2021 20:27:35 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
