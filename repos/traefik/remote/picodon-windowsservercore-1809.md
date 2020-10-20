## `traefik:picodon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:001b90239121ce99ff089cdc60ed0007d6bec5e1b21ed77006115d8ed422a329
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `traefik:picodon-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull traefik@sha256:5d7e16f39dd178b8e708865a339ddaa669ecfa6c7b7a1353a76eaf7527bc95fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2408551936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe53096686685c8c496a730f0a1adda7e75f66d54d1c6fa78ce0bf9947937a7f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Oct 2020 18:16:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.3.2/traefik_v2.3.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Oct 2020 18:16:03 GMT
EXPOSE 80
# Tue, 20 Oct 2020 18:16:04 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Oct 2020 18:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bdd186e1a3250546acc53e640313f116641964b7fdc15f000c5f3d8e64dae`  
		Last Modified: Tue, 20 Oct 2020 18:17:08 GMT  
		Size: 34.5 MB (34457274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64cc0bcfac67ffa0c35200bc99a52d4894e041c85cc081bea7f6f917452e0bb`  
		Last Modified: Tue, 20 Oct 2020 18:16:28 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a424c26b77a039045583035b9762e58d5feeb9a0ff782de51d19541fa33a004`  
		Last Modified: Tue, 20 Oct 2020 18:16:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a36bd478654021fdb2d16202816d63ec69be53ffc1f1f32b5ec0b60eee5b437`  
		Last Modified: Tue, 20 Oct 2020 18:16:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
