## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
