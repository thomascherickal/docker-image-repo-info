## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:17a6117b4621e8c252448c0014078eb939ce7f9d79f926cffd1cb6a33e761665
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull caddy@sha256:2e9857a82e1d67d71abe0de2b0773284aa0bb6d11bbe0b2160b3d4f2dcc8a812
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1955030028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90ef7e3fd9125f5df4ff4cdad1e7a56ba7159de337f77b82f5173b07ab94313`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:42:14 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 14 Jul 2023 00:42:15 GMT
ENV CADDY_VERSION=v2.6.4
# Fri, 14 Jul 2023 00:43:23 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 14 Jul 2023 00:43:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 14 Jul 2023 00:43:24 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 14 Jul 2023 00:43:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Fri, 14 Jul 2023 00:43:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Jul 2023 00:43:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Jul 2023 00:43:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Jul 2023 00:43:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Jul 2023 00:43:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Jul 2023 00:43:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Jul 2023 00:43:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Jul 2023 00:43:31 GMT
EXPOSE 80
# Fri, 14 Jul 2023 00:43:32 GMT
EXPOSE 443
# Fri, 14 Jul 2023 00:43:33 GMT
EXPOSE 443/udp
# Fri, 14 Jul 2023 00:43:34 GMT
EXPOSE 2019
# Fri, 14 Jul 2023 00:44:29 GMT
RUN caddy version
# Fri, 14 Jul 2023 00:44:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bb4f1e513e5b8067f0b87accb23692464bc0eb6d0b33abbdab5d3ba562731c`  
		Last Modified: Fri, 14 Jul 2023 00:54:06 GMT  
		Size: 456.1 KB (456146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4254b85bc800cd3c6ac27302489d67e69720482341903662f497236bbe0ac0`  
		Last Modified: Fri, 14 Jul 2023 00:54:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e2003eb358f3acca4f74b748abe497fe7537f1803403e594fc9bff212d05de`  
		Last Modified: Fri, 14 Jul 2023 00:54:09 GMT  
		Size: 14.6 MB (14605794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b89f5b77b4053906225dd11e08bd26110b42723d8abca77a5ad77e02c89f77`  
		Last Modified: Fri, 14 Jul 2023 00:54:06 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5ac60357799f560e1db0bc846285480070cc13a6dbf71f5c889805c2735911`  
		Last Modified: Fri, 14 Jul 2023 00:54:04 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f87337e64000cf59b22f04f6637df09e2b859c9523d1fbdf3d5d4c966937cca`  
		Last Modified: Fri, 14 Jul 2023 00:54:04 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649be33b1f8a2618a81a18eeb53f4b5dfa19dd90ca54b01baadced70ec53154b`  
		Last Modified: Fri, 14 Jul 2023 00:54:04 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23177fa76705d8fe43daf0e31999414acaebc05c4ffb920984e8c77b29087bd`  
		Last Modified: Fri, 14 Jul 2023 00:54:04 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647d13417da95d1100ea5338df882bd2a978bb38760d2c88639af8cc571efd3`  
		Last Modified: Fri, 14 Jul 2023 00:54:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dd5ebd8fa20ef3105f651938a5208ddb140c5f0000544345160c2a601af71b`  
		Last Modified: Fri, 14 Jul 2023 00:54:02 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed75ed571a82157608e5159b80cd06454b3680c9de4d58df8e1fbd13e19f0eb`  
		Last Modified: Fri, 14 Jul 2023 00:54:02 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a7f1c4fa9043a0fb483d2fae4d69f10ffde8c1f62ee759fc666b43cf2a2ed`  
		Last Modified: Fri, 14 Jul 2023 00:54:02 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadec124c4a0632727854120970ffc0df7ece67add4cf1de81b1f3748058e700`  
		Last Modified: Fri, 14 Jul 2023 00:54:02 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a56c15b23cd77f0e5d901496518ac9b4ee8a417c7aca40e6d2c161189d20a5`  
		Last Modified: Fri, 14 Jul 2023 00:54:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506e5f0d549ef21ca8a52ef08acbd1fcab5a53d0b9a5e8d586c34a2fc662e5bf`  
		Last Modified: Fri, 14 Jul 2023 00:54:00 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480455d92ece3f0a484510fbfe5258b8d6f851fb46b029f3af20503e6ad994a0`  
		Last Modified: Fri, 14 Jul 2023 00:54:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a47aeee7e0c0053a1766afca8f0de4363ddb3da3d939f4a4db43a237c7870f`  
		Last Modified: Fri, 14 Jul 2023 00:54:00 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d74b6e3eff6265366317d8040305f6893ee57d24ab94a78fb753cf83bac3f`  
		Last Modified: Fri, 14 Jul 2023 00:54:00 GMT  
		Size: 255.3 KB (255268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcd428955520870b11d2931e94fcd4fc23b9703d9adb2605d15e70e30714ae2`  
		Last Modified: Fri, 14 Jul 2023 00:54:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
