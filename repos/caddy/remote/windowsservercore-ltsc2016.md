## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:15e5d6e48e5705c59d244d4506d9259c37b03f6ce2a15bed80e02c1e533ad2ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
