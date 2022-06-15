## `traefik:epoisses-windowsservercore-1809`

```console
$ docker pull traefik@sha256:269ccdc193d1f97affbf2a3baa17c28d4b4324addc7b484ee1016856673c0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `traefik:epoisses-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull traefik@sha256:7533a8b4b3d39289724a71b1d3ab40438be7464e7a6cc099ae023413fb65e0f3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691410794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e85adc1ce7628a3b37bd34d2ac03995dd9882f7166b9250b8d48b02872b510`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:57:11 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.7.1/traefik_v2.7.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jun 2022 22:57:12 GMT
EXPOSE 80
# Wed, 15 Jun 2022 22:57:13 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jun 2022 22:57:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.7.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b198525252836b1340587282e9005608f8a92c20d8b7b7013d61738228a48800`  
		Last Modified: Wed, 15 Jun 2022 23:00:08 GMT  
		Size: 28.1 MB (28125336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074082ecd440c9a6d6cf70db58a8bf9fe1295e6499bf66ce440f94af264e173d`  
		Last Modified: Wed, 15 Jun 2022 23:00:00 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab22aefe2724449fc17db0174409ae893ae145376b865163809011ae1b90f879`  
		Last Modified: Wed, 15 Jun 2022 23:00:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2319a1991613a9acec284922506e3853fd153c67dfc81d6382c9a8dc16390d`  
		Last Modified: Wed, 15 Jun 2022 23:00:00 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
