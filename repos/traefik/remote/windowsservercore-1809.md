## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:fa7779f5328c4db74250ab2932a6709ff1db6a521b29686d3b8965e0804acfe2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull traefik@sha256:bd18911c8994e17fda72e1e3a91ffb976423621f03f0ebe9bcb6461ff1452013
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2739268945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015c11c14de18ddc5b5d6e957400b5ee39292dd83b91c5a55204e15957c87f5b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 19:00:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.6/traefik_v2.5.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Jan 2022 19:00:57 GMT
EXPOSE 80
# Wed, 12 Jan 2022 19:00:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Jan 2022 19:00:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f149283492dc638b2397be23be317a545d1ce2abf323b0aa67c667da3dc50a`  
		Last Modified: Wed, 12 Jan 2022 19:03:50 GMT  
		Size: 27.0 MB (27032373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33edf3d8e965212700573968bf1a935afc3017fb8ee109c01dfbe564b5ad800e`  
		Last Modified: Wed, 12 Jan 2022 19:03:43 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240404b2405746a2f6f96d51927cbd3854aed54967766486bda67ff05f2f0433`  
		Last Modified: Wed, 12 Jan 2022 19:03:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d69e79955a7725160a6c117c2b0d62e23c08d83355c51ccf8e3817ddfcf5e4`  
		Last Modified: Wed, 12 Jan 2022 19:03:43 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
