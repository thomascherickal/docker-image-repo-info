## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3ebcc75c760fd3f09c9af3a083679243b86e38acac6b9c87d426f5e060bb5e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
