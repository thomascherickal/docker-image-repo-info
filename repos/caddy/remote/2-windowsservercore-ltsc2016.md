## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:971ecb6797495e16d5ee3ede15138f5ceaee0930af2ee0b6fbc9dbae848302fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
