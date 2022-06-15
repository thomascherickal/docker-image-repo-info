## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:38d6b6a109eefba8100d1c9f39cbc3f2cbbc65414bd9d4c21a3f3d3803a20e70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull traefik@sha256:fbdf20663eef4b356b91897c11768e710fe5d8c0a20db676b727ace282010c05
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686129323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2bff99d35ce807fc8be468d820b698c0aa96bbc198d8fe2d862f033d3a872a7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:58:35 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jun 2022 22:58:36 GMT
EXPOSE 80
# Wed, 15 Jun 2022 22:58:37 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jun 2022 22:58:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9c081bfa67f6b18ab023e3e6f245649e859bd7f6def8eda5884371448bdfa11`  
		Last Modified: Wed, 15 Jun 2022 23:00:34 GMT  
		Size: 22.8 MB (22843843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10edb73d57df6d226de72153277ac47e944dcef4eaadebb4017ed7c9b748699`  
		Last Modified: Wed, 15 Jun 2022 23:00:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0a0dfe9477fcfe1a48749ca97bceaf457e5fb84a996d15fd78917ee6ce177f`  
		Last Modified: Wed, 15 Jun 2022 23:00:27 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12f9f231fd68bd6cc2c7fab6929a79a59f1df6127ef65cd3a70c3fdd2d84a92`  
		Last Modified: Wed, 15 Jun 2022 23:00:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
