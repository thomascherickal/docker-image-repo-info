## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f504e734712cf31dc0903f54de87aa8791a825b7894d33a007da91b42a178a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
