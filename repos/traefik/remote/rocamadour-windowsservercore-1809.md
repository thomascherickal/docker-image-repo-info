## `traefik:rocamadour-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0956c5f848a9384b3ef1eee79636c8a696524ef606f5805df1bad274dbbea9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `traefik:rocamadour-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull traefik@sha256:6210ef2c7c72b8964cc386dfcfacdce26c85c70dff5a5ff7945d5b609fce9db8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2739467068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ff1823a36bec73830ecacd8ae8cfcb48575ff8c395e7eab607958552d839c70`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 18:59:26 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.0-rc1/traefik_v2.6.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Jan 2022 18:59:28 GMT
EXPOSE 80
# Wed, 12 Jan 2022 18:59:30 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Jan 2022 18:59:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4edda45412809b497b821e17d7f7f8356b7f57cf9c8de5126b6264b901a381a1`  
		Last Modified: Wed, 12 Jan 2022 19:03:26 GMT  
		Size: 27.2 MB (27230479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4a42924c3c2874935717ef995abb924d2322319265c5b3c3896c56bc15e8af`  
		Last Modified: Wed, 12 Jan 2022 19:02:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7509d36cca44f18b4f590dcff7eab7768f99bdbf36672dba09f19ffe1db09c`  
		Last Modified: Wed, 12 Jan 2022 19:02:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6703b20438c70382d6b9c25ca780d620fe640e9672d2a7ca85def37661730bc5`  
		Last Modified: Wed, 12 Jan 2022 19:02:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
