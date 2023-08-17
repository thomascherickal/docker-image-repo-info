## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:9b2d0e89dc4f5f508ec90143d8b6b6d2cdbe9067fea9d0930cbb9812eb816b01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:8d641d87b059de975dc94ff579d47434e347b333b33a4a8f15cd679c062a14c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011934670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b2ad9f1a3657d84dd869da76d22704a2848d4a92f831acbfef09e26e80cc6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:16:58 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:14:59 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:16:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:16:14 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:21 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:22 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:17:19 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:17:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d698e8ba8bfd4c31116f0d2c87cfcf2ff17baa1a5c678b116b3aa1ac8ed73d`  
		Last Modified: Mon, 14 Aug 2023 18:23:17 GMT  
		Size: 483.6 KB (483626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcf545f7c90cab6f6962d3099898462129da2e6b06a80802d52ff1e9d2fca08`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ecc8b4521923b522dd6392a862d0dff9edd10c1e3b520de8f130de2170880`  
		Last Modified: Thu, 17 Aug 2023 22:21:16 GMT  
		Size: 15.2 MB (15201779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ddd9c690b84a4a4744ec5ac91059e12e1aa92378220080fcfbf616c59b4c26`  
		Last Modified: Thu, 17 Aug 2023 22:21:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63adbcb9cba5e8d67eac5e059c7bbb9dfe3040f0933afb5e1f8cb7d4c211b4a`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e15ff22938f514e6118606619ff28e9e5ee145d6f3dc6de1de62ea4051575c1`  
		Last Modified: Thu, 17 Aug 2023 22:21:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438a6cab105b637f625a3fd00d7ecaa6792ad5dc120bf1be36e7d6e19ee44b4d`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfd206f96497c8e0730c72c36ecedea57379a6a219903785dc1478b50b3945`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e651df7142dc872814a59faff8cf791ab4e4413ee6a9b043fe02a2af9da24fe`  
		Last Modified: Thu, 17 Aug 2023 22:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7f62d857ed7e15d08d52d1ef08f3c21e25751d17e8a5418c02f6adc366eab`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6347f1227dc933d98b8f02d22cd440529284e7c8e415e96cee265ae2c7445b3`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776f9f89b2242d27c9c49da3465d2ff6acb224dd3315837bda709f3fa0aa4ff`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaab02f29add47735607e798c40625216306d00d57988d1ece40f43b93f706c`  
		Last Modified: Thu, 17 Aug 2023 22:21:09 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed26555e0c9e51aa5dbf4125ef3ea56c6d84274b4d8160ce10c3c0d9e7106d`  
		Last Modified: Thu, 17 Aug 2023 22:21:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c0484ea6d941786f507e72c143bd1c64d4c42bcd773bd745330a55b89d356`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07137395441a56a870d882d84faac751156b0486c6528fa18b6d706ff250d8`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2950cf3d51ba47c2b41415fccf9b67e813735f67ccc34a0ce5f1a1a4a34e56dc`  
		Last Modified: Thu, 17 Aug 2023 22:21:06 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25de03b5a8b8f2752cde31b881d457ec5900438b781cc65cda3aca9444b2377f`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 269.9 KB (269882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f3d70fb1dd11e79f9128736ada85993e1b4fd603b2f8164aac49ac1efda548`  
		Last Modified: Thu, 17 Aug 2023 22:21:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:f4791cb0179b98b28e760842405262d782735176b147c84f26709bd1361c8798
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813299019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b759bf39605cbc0d0ceaaa8eda1623452b1acd67deb11c0d22defff59f2058`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 14 Aug 2023 18:19:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 17 Aug 2023 22:17:27 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:17:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 17 Aug 2023 22:17:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 17 Aug 2023 22:17:56 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 17 Aug 2023 22:17:57 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:17:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:18:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:18:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:18:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:18:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:18:04 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:18:05 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:18:06 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:18:21 GMT
RUN caddy version
# Thu, 17 Aug 2023 22:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c23e01ee014d9e05e276268c94980b00a0720fcb5488a368b20ee74701ed78`  
		Last Modified: Mon, 14 Aug 2023 18:23:42 GMT  
		Size: 461.2 KB (461170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8a7576f0b2ff121a0e9658821e52a7b356abbd90c9215b750ab7fc2127f6ae`  
		Last Modified: Thu, 17 Aug 2023 22:21:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ecc6db59a89a0a9f61364702d6af7202fa4f3f742ec6dff93c3a5b53e3826`  
		Last Modified: Thu, 17 Aug 2023 22:21:44 GMT  
		Size: 15.2 MB (15169088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9323e4528d7a59819754484fdbeb047240a6f1f0dd262b734a226a4249dc0a0`  
		Last Modified: Thu, 17 Aug 2023 22:21:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3a3b69dd93b979cdcd1e0759ee1199bc8d5a510a6ce9bca3856201d747468`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ce33676578802911228ae7aba31fe1898897ede8c69e12a0959a37a11d130`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896eeb3f2c45b2bba4fe5e5da02be1289c4cabcf574a38c19d1616ebf552d4c`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6563dd3d5f912ae2b7bd629d2dc731df89b1dd107e2cbb85dee24a0d5c550a1`  
		Last Modified: Thu, 17 Aug 2023 22:21:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420011263062842c72720998f13fa245d9bef077622fde4e17cc60cef3e00bce`  
		Last Modified: Thu, 17 Aug 2023 22:21:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2385fc0cb7a281a35df415654aba711bf70fa23b963faf0a3f0055d760f5c41c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a58351f25f399f8a9399e60dd315cd8c695972a9e51f2271e3377151cf621d`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506eb3a97b70fc7dc1c1c3464a89512890cd48c354658e58e61d5acfee63f1c3`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf8c25cfcaf858db6ffd2630a26ca3a13ad2fdc941a01438ea9ea80ccb20c`  
		Last Modified: Thu, 17 Aug 2023 22:21:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcedddef9863d16c4d713280050f604b44968bc253844c27e46cb8871eb17a99`  
		Last Modified: Thu, 17 Aug 2023 22:21:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01313141e38a9b2b15a3e831a2d11a3eb47611bf99b0677be3c49693984f64`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504a80bc0f7aa0c98a143033f551be8fcf0653046e7313c0de080b82ad97ad52`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280053e45030e2421ea4d1cdfd721c24f40d30518b1ce8af7e0811363daf6eca`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0d07466cd8f053bf957a35cbe340d419f5c2f6ff48565bb8a5b255998e3e94`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 280.9 KB (280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad52776067d7be890960cfd7082041a93a802b96fea6d31fc724192c49eb00`  
		Last Modified: Thu, 17 Aug 2023 22:21:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
