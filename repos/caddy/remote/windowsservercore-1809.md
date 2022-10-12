## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:6caf3e51db510e1b1da9e7fbc854fdf0e6b120f6990d166ad4493dc5a25113de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f0d631ffca11e52e8533977f470a1a7b629ec530277bcc665da39f1f1ce3e4a1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726726610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6988b435ab1d559c88e0ab2ae19de6ada3831d3a38e1560bd4ccb62245ee74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Oct 2022 16:58:31 GMT
ENV CADDY_VERSION=v2.6.1
# Wed, 12 Oct 2022 16:59:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Oct 2022 16:59:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Oct 2022 16:59:36 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Oct 2022 16:59:36 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Wed, 12 Oct 2022 16:59:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Oct 2022 16:59:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Oct 2022 16:59:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Oct 2022 16:59:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Oct 2022 16:59:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Oct 2022 16:59:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Oct 2022 16:59:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Oct 2022 16:59:43 GMT
EXPOSE 80
# Wed, 12 Oct 2022 16:59:44 GMT
EXPOSE 443
# Wed, 12 Oct 2022 16:59:45 GMT
EXPOSE 443/udp
# Wed, 12 Oct 2022 16:59:46 GMT
EXPOSE 2019
# Wed, 12 Oct 2022 17:00:35 GMT
RUN caddy version
# Wed, 12 Oct 2022 17:00:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6918ef6addd5831c9fb734e80c07d77e76d8341f12e80e0b45fbbecb726ec3db`  
		Last Modified: Wed, 12 Oct 2022 17:04:33 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637460689a42f5dbdff404a6c3978a098e69b28dac2b0540fdfc0f0efdcecae0`  
		Last Modified: Wed, 12 Oct 2022 17:04:36 GMT  
		Size: 14.9 MB (14872825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53171eb2725db81963677560701632565f0a71cc16092173ac0e950bb9082a02`  
		Last Modified: Wed, 12 Oct 2022 17:04:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc91b3cae46cfaaf5c5fcf444fbfcfbf6e8022a3bf9d9be8535c393fe7d26c`  
		Last Modified: Wed, 12 Oct 2022 17:04:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864a124d0d06b1a5d074f5fc5c029e56f9bd5f7ace5b8f9908b784ab93299eb4`  
		Last Modified: Wed, 12 Oct 2022 17:04:31 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150de7a7e94689dbb4a0cd5bcbd1b648dbffc4ce7c54a67a4a6d884e9579295`  
		Last Modified: Wed, 12 Oct 2022 17:04:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c0c202c5b4ec2c240e5b7bd3b41d3bcccc6a71e3309973b7496fab6f56ceba`  
		Last Modified: Wed, 12 Oct 2022 17:04:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d24b725acab1fd5e9d064846f23956f0f5cdf8ecdfdf1cb9e3c092a9c1105d2`  
		Last Modified: Wed, 12 Oct 2022 17:04:30 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513fbef87a84cb9a30d724de110e0b7cf27bde267ea90db4361bd897a8964541`  
		Last Modified: Wed, 12 Oct 2022 17:04:29 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe5bdceccd2927113ac968027e59f05940f678e818c6fcdff70dbc5c1a46c8a`  
		Last Modified: Wed, 12 Oct 2022 17:04:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9de8c7752e0f9112e5f8e470f85a5ad3efb80ff8ebed8412aab7488e7b5f5e5`  
		Last Modified: Wed, 12 Oct 2022 17:04:29 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae88e2f8f3e48b60c35155585a7e99d7b4adda3dd445ed8217d09402ddf1f311`  
		Last Modified: Wed, 12 Oct 2022 17:04:28 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f161fc113e06367a56fa5183b1944c91e8fdc0634f5b3185cf558a80e35d03c5`  
		Last Modified: Wed, 12 Oct 2022 17:04:28 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a209ee80b3933d5238c64b54a15739eb5ab8984f6ba245299956136f2e8909`  
		Last Modified: Wed, 12 Oct 2022 17:04:26 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7665c04caf810b8036306fe55d58e6a9b9b8bfe1b12579429f16a4721b1037f`  
		Last Modified: Wed, 12 Oct 2022 17:04:26 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591ee317359daf5db1dc085f26aea3d4d878839ce909a53d08d141b26d212b22`  
		Last Modified: Wed, 12 Oct 2022 17:04:26 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaee89258120a6b80af10b44b00b33d39e90240058a095c5425b307e8b6df4a`  
		Last Modified: Wed, 12 Oct 2022 17:04:26 GMT  
		Size: 307.6 KB (307571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfefd11ed1a4df24244ad94b57aaf31a6ba02cecdcd0686ae6a7e86688a4189`  
		Last Modified: Wed, 12 Oct 2022 17:04:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
