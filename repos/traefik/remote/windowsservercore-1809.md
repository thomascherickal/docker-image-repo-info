## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
