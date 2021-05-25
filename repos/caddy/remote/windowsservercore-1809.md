## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb9fcd910a8050aa2ce11ac6b195722843c6efc46c1cf68fbb3a4172914c2e30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
