## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:c425c63e4e236cbe5bee3492948f73aa85142a1392096f56c9e952f6cfc61364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4583; amd64

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
