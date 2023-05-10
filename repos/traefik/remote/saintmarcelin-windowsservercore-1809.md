## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
