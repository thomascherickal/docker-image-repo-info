## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:d197841c98f70a5cfcc3aae372d7843eff10045fe38cdadcc5acdf2fd084fc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.1040; amd64

```console
$ docker pull traefik@sha256:6ef62e89404c45ea849cd51a5dcfac5732a225572b7fd1679f9345ab21577a7e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2254677851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b8df80a5f009f8eeeba97b27d2069784c291ae48289a714a113adbb942941`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 28 Feb 2020 23:24:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.6/traefik_v2.1.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 28 Feb 2020 23:24:15 GMT
EXPOSE 80
# Fri, 28 Feb 2020 23:24:16 GMT
ENTRYPOINT ["/traefik"]
# Fri, 28 Feb 2020 23:24:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76f678ce4ee0ac830ca2fbfbe9bb25345f876cbb007fe9683043f3cfc54411d`  
		Last Modified: Fri, 28 Feb 2020 23:24:59 GMT  
		Size: 24.2 MB (24169151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48efb386c689e1ece2ee5afa2b9c2a40d015e2bd1fe8166fd5e785b2402b4d7b`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b37b2b9555ab0edb0fc149d4c974e6bf124c14c385605002d75cc7521955b00`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06a84dcfb78e0a621d3addfd89ebdffd9763f973134ef5433195c6b49c6f33d`  
		Last Modified: Fri, 28 Feb 2020 23:24:53 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
