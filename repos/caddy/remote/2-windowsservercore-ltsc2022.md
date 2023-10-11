## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:370b283a915adaa0bde053be26e8b655ba7af9fe85c866ca3eb9536faddfb246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:35a8490a9e968ffb0e52546066de74169e5bc047efbf00c4f5b84d14b797b320
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875800819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab570e6f42bf1067f0f4f5d8ef4929ef28487a5146036a777f9cfd3da4ed119d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Oct 2023 04:02:07 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 11 Oct 2023 04:02:32 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Oct 2023 04:02:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Oct 2023 04:02:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Oct 2023 04:02:34 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 11 Oct 2023 04:02:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Oct 2023 04:02:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Oct 2023 04:02:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Oct 2023 04:02:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Oct 2023 04:02:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Oct 2023 04:02:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Oct 2023 04:02:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Oct 2023 04:02:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 04:02:41 GMT
EXPOSE 443
# Wed, 11 Oct 2023 04:02:42 GMT
EXPOSE 443/udp
# Wed, 11 Oct 2023 04:02:43 GMT
EXPOSE 2019
# Wed, 11 Oct 2023 04:02:57 GMT
RUN caddy version
# Wed, 11 Oct 2023 04:02:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccd56304cba26238d4c5289d3c27378fe3fc13d558af959244f596a849f6f93`  
		Last Modified: Wed, 11 Oct 2023 04:06:09 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d333191d07db1d95e40f080cf13b1a625e28a73403bedd38fba9facc6df886d1`  
		Last Modified: Wed, 11 Oct 2023 04:06:12 GMT  
		Size: 15.2 MB (15176630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b72797a791127785307b1c8d764ababa71697ed89f57502a0aabc0c8eb8a7f`  
		Last Modified: Wed, 11 Oct 2023 04:06:09 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cc3bee4a9cb38d59ae2d90b8e11dac2b71f1d80c094cec4aaad0c4ef8fd047`  
		Last Modified: Wed, 11 Oct 2023 04:06:07 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a748f0c12ebcfec93b27c46ee63ac1bbd4bbb0aed451ce8bf1d4572e776594`  
		Last Modified: Wed, 11 Oct 2023 04:06:07 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235657d150e797ad9931513299814ff77b75b190efd14f05fb58c7e71fbdbacc`  
		Last Modified: Wed, 11 Oct 2023 04:06:07 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79c4cb9149a67e918d014ddebaf3747bce0610526a08116a4b7efbff28c89c7`  
		Last Modified: Wed, 11 Oct 2023 04:06:07 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eaf5c52e58dad960d0ccff695470b0e6afc54bb124945468e2d30de79082f4`  
		Last Modified: Wed, 11 Oct 2023 04:06:08 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90f4bb67c1f3c87bbfee31addd4e0ecf20035d9b1242dd2295bf5ef104f133`  
		Last Modified: Wed, 11 Oct 2023 04:06:05 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc7345c29286429486f87f5e8cf61f72a3ea9a6d3eb44d2657746243504bbc5`  
		Last Modified: Wed, 11 Oct 2023 04:06:05 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3393907d296576137be888e66fe0a4e0582e0074be6dda5406ad48347d33da2`  
		Last Modified: Wed, 11 Oct 2023 04:06:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb1867d35c87a9740398d049f5c54b8f6ba42039509134ce2cdfebcbb03603c`  
		Last Modified: Wed, 11 Oct 2023 04:06:05 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68a8d8df9f3407805ef8fe2454d3855d2c97d57b027d5cb121b0e123cddfce4`  
		Last Modified: Wed, 11 Oct 2023 04:06:05 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5518bb1a09918491b070980da608f4098156a4403d36970a7f1eb754bdc8c28`  
		Last Modified: Wed, 11 Oct 2023 04:06:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d6ad0f9e121f64bf2a9f13c51d26b84e39a1260d7a7fafffa2e90b3c48f94d`  
		Last Modified: Wed, 11 Oct 2023 04:06:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2376a20c5922b82ab080bc0ccb5c8793b8fe27cee3d9a0781a9c6e97b9b1085c`  
		Last Modified: Wed, 11 Oct 2023 04:06:03 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c822245a1f51dd6309c39d231e80da13629a04170e7438435ee6d2fd388c6f`  
		Last Modified: Wed, 11 Oct 2023 04:06:03 GMT  
		Size: 289.2 KB (289182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d03ccff4d911b212ed869adfb8e487be716708de3bb523a291719f2c1cb95f7`  
		Last Modified: Wed, 11 Oct 2023 04:06:03 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
