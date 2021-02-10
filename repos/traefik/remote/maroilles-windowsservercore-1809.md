## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
