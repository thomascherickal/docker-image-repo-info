## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:48f63da0fbf6ae81f0a92530e92b8f9a0756247f0119461c9ee76acf610c6f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:89e85aed85700177e047f93b44d2782deafacbc159abac54dddbe571d1853a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698696531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10c266e4a75a171ccf01e74e31cd01097f5acaadc2b783c37f49beb49700efd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 21:01:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Aug 2021 21:01:17 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 11 Aug 2021 21:02:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Aug 2021 21:02:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Aug 2021 21:02:23 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Aug 2021 21:02:25 GMT
VOLUME [c:/config]
# Wed, 11 Aug 2021 21:02:28 GMT
VOLUME [c:/data]
# Wed, 11 Aug 2021 21:02:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 11 Aug 2021 21:02:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Aug 2021 21:02:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Aug 2021 21:02:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Aug 2021 21:02:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Aug 2021 21:02:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Aug 2021 21:02:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Aug 2021 21:02:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Aug 2021 21:02:50 GMT
EXPOSE 80
# Wed, 11 Aug 2021 21:02:53 GMT
EXPOSE 443
# Wed, 11 Aug 2021 21:02:55 GMT
EXPOSE 2019
# Wed, 11 Aug 2021 21:03:47 GMT
RUN caddy version
# Wed, 11 Aug 2021 21:03:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b830acdcbafa43b359c2bde9b47eb96343b52f7804ef5497cd73e88f92462d7`  
		Last Modified: Wed, 11 Aug 2021 21:13:45 GMT  
		Size: 369.2 KB (369192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75ca7a3313f0dd0ac58266bf97b777b2d0c4ee206806cf3b35207eec48bf121`  
		Last Modified: Wed, 11 Aug 2021 21:13:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd236fbc21e47110f7e207157d2e94056f454de928ef7e1e523c75f307d94c8`  
		Last Modified: Wed, 11 Aug 2021 21:13:48 GMT  
		Size: 12.0 MB (12002585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3dfd9204a4c06d07268f82b0c8f30efa2078f5c102f05dea0139da10cef608`  
		Last Modified: Wed, 11 Aug 2021 21:13:44 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b09cae1e2193616e62f32f411a35ce228ba18dd8365af4e0f9384b1d18e4cc`  
		Last Modified: Wed, 11 Aug 2021 21:13:44 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f90022eda80c8b7a26bce585b23e07ea6127bf1021b51c33d9a479cd8aeb7c`  
		Last Modified: Wed, 11 Aug 2021 21:13:41 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be293839008c6deb19527ad8f4b696a4a9193037d9691adb4956bcade39f22fe`  
		Last Modified: Wed, 11 Aug 2021 21:13:41 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a1003c9e86bfc434bb6412c3a4844e298ea7d8cd28eef9245b9857139b520`  
		Last Modified: Wed, 11 Aug 2021 21:13:41 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c4be7b5209e68145aa86f7cdf863e72ca42fb66d507eeb0a65430eddc11e6`  
		Last Modified: Wed, 11 Aug 2021 21:13:42 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea471cb078ae91803e575f58b0d61fa4c9c34b9035d566d0e8edeeecfb4b5e6`  
		Last Modified: Wed, 11 Aug 2021 21:13:41 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25ef2c8e2d85775b45ac2abfd5ae15e4c44dd09ca8bc2f738e02a40a5757420`  
		Last Modified: Wed, 11 Aug 2021 21:13:39 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdaca1b8f26dc7d6c4da2a5c4141cedb743033057b2c3dad777c3abc61c9d60`  
		Last Modified: Wed, 11 Aug 2021 21:13:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c87194b1226f3e016b6c05613e3c2c69155ef32589615ed1261ed7ac896752e`  
		Last Modified: Wed, 11 Aug 2021 21:13:39 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654bf713dae5355c49e2241ca7108171da00511b6268710d0bd3889830ea5a3`  
		Last Modified: Wed, 11 Aug 2021 21:13:39 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607d1551a8d55cdae9dff0ef8c551906cb53f109ab5d5d4218a595b5c7b0515d`  
		Last Modified: Wed, 11 Aug 2021 21:13:38 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2993a18a9cbf7b3df3d20ab0103a27214e439f25c60b912472a6909f7e21bc55`  
		Last Modified: Wed, 11 Aug 2021 21:13:36 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf93ac4f5cee5f1e2e1d1bc8481718c07af0214103ce9b1811cb00d8e63f1106`  
		Last Modified: Wed, 11 Aug 2021 21:13:36 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516eef333e82a1131009a68c0f4c8175152a5b0a82070ae2608e9abbbdbd343`  
		Last Modified: Wed, 11 Aug 2021 21:13:36 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da8f8a86929c4ae3e98f5994d04e0c1aebd80816bda1141c7c32b8172f0d328`  
		Last Modified: Wed, 11 Aug 2021 21:13:36 GMT  
		Size: 301.3 KB (301311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6cec0f0cff82c0cd5bb06544db161836ba382b900534e5a30fc7929e5c85d5`  
		Last Modified: Wed, 11 Aug 2021 21:13:36 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
