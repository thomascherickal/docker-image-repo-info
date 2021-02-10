## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d0f4e57b0d1eb564339e530b53af4390b6d7897bbc4cf11a42c685136eaf732
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:e5c4ad0b5705bd261acd6f6543a3e18bd175f6d2c80189e54be0923a9b014fe7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474612363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67df6161182e4172880409ed0a1c806cad8585ce225de0ed5c08d53e34464a0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:09:35 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.2/traefik_v2.4.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 Feb 2021 20:09:36 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:09:37 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:09:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cad6fab76bd2d216233399db65245f842d3b48b5efe843664948486f056383`  
		Last Modified: Wed, 10 Feb 2021 20:11:30 GMT  
		Size: 35.3 MB (35340091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6bcd396adbef67e530b0a69d1f5383c7fa8b5e1a43b41267ce0d1ce8514698`  
		Last Modified: Wed, 10 Feb 2021 20:10:49 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756640a0c1cbbaf49818590afb239d38cba4c223dd5b48ffe6378eb454d9f88d`  
		Last Modified: Wed, 10 Feb 2021 20:10:49 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b210277da2ff5834ddb94790729fdab8c8ff1690db067371c9ad27ea9554338`  
		Last Modified: Wed, 10 Feb 2021 20:10:49 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
