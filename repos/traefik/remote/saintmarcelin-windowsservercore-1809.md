## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1393f9c11a3149243b88f0d07cefd51a9c9b44b7960d67552c9be9c071b69882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull traefik@sha256:f0eb7783d8cd021cafb91e818cb29588e8b595bc7bdcb399db491c8f94a9a6fe
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2108904623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1561c20d7bcac22b318db74bcb2333000cd1cfa143326efd83a57d5011e770be`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 07:14:48 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Apr 2023 07:14:49 GMT
EXPOSE 80
# Wed, 12 Apr 2023 07:14:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Apr 2023 07:14:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1f16f157060a7e00599b02c38abf2b7224822e6e67a5f8e831881309e9bcb0`  
		Last Modified: Wed, 12 Apr 2023 07:17:29 GMT  
		Size: 37.6 MB (37607971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b898212a0f06d63dd0f87e4ef8270848728f54244d0e45482b3363ce094a71`  
		Last Modified: Wed, 12 Apr 2023 07:17:20 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1596141349ee66b30d8060b045b3248ac5efd19c2c7afab6e0bd9fa165c79cc`  
		Last Modified: Wed, 12 Apr 2023 07:17:20 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b971e5e170a9a5338840982c9a4700a63560006440129aa8e717440b213101`  
		Last Modified: Wed, 12 Apr 2023 07:17:21 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
