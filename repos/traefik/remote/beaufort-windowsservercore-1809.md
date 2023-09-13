## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
