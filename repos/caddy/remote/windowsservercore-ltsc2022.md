## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:05ced206e45b045bc5cd525d92a16ed5dc3db97b7917edef04152739d06b712b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull caddy@sha256:8b2e9ac9b72c8b2c90bc15116cedbb8044d599e4f86ffcbb48cebdfdf97d19f7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1905326657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7092fad7c71072036e6f6e418de96b9a293b2a5fa6c1f533192cee80981c2fdf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 02:33:55 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Dec 2023 02:33:56 GMT
ENV CADDY_VERSION=v2.7.6
# Wed, 13 Dec 2023 02:35:10 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.6/caddy_2.7.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b2321473be1da500a8f6e4276aed03b11946e3758b792a3e9ba50c07246456d64d7da931d6d58be43e6d3cfd07c1ad68f6838df8e090bd5d212224a9bf94daec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Dec 2023 02:35:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Dec 2023 02:35:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Dec 2023 02:35:12 GMT
LABEL org.opencontainers.image.version=v2.7.6
# Wed, 13 Dec 2023 02:35:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Dec 2023 02:35:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Dec 2023 02:35:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Dec 2023 02:35:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Dec 2023 02:35:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Dec 2023 02:35:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Dec 2023 02:35:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Dec 2023 02:35:19 GMT
EXPOSE 80
# Wed, 13 Dec 2023 02:35:20 GMT
EXPOSE 443
# Wed, 13 Dec 2023 02:35:21 GMT
EXPOSE 443/udp
# Wed, 13 Dec 2023 02:35:23 GMT
EXPOSE 2019
# Wed, 13 Dec 2023 02:35:42 GMT
RUN caddy version
# Wed, 13 Dec 2023 02:35:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c853ded9068434b9128a8016b3ae5e18f748f62801c7bb6e6092495300ec`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b76d3c17fb1ca1499edf5a0a7fe2ed357de61bc5478580af8c193d8c59e8139`  
		Last Modified: Wed, 13 Dec 2023 02:39:22 GMT  
		Size: 468.6 KB (468557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b9bfc982e2d76e931acf88ef85dfe1c943d4412d8e0abc82f7f0837e3ffe`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be685bdfb2389b99d51da84fb605d5905240fb7fbb82779d90949871c42c3a01`  
		Last Modified: Wed, 13 Dec 2023 02:39:24 GMT  
		Size: 15.3 MB (15270636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9935999a24844b91a4364fda0be1e1ffa280fb0c3c3c51157ffee05dc396bc2`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bd056752e2fad4d5b1e26bda93daeb2e2b89b03fc440f547e8e8e57b56ec54`  
		Last Modified: Wed, 13 Dec 2023 02:39:19 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bff69c07007af0ff21680f637729be4b8d66a9b114305a47b54b631e499932`  
		Last Modified: Wed, 13 Dec 2023 02:39:19 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8602ee7f30c15eb312beb9be91c2987f09264a3ec61fab2a25f7388c80361e65`  
		Last Modified: Wed, 13 Dec 2023 02:39:19 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d98bd6b64e0a8382fcdef83a12bb138867f39b06a481c87d92f5e8b6bd637db`  
		Last Modified: Wed, 13 Dec 2023 02:39:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dab994312751dbeec291009c1153b38cf3621f929570200eefc6f838922099b`  
		Last Modified: Wed, 13 Dec 2023 02:39:19 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb56c650abb1c98df5455b6b8c1864695f45548b82de29e570ce3f46299e574d`  
		Last Modified: Wed, 13 Dec 2023 02:39:17 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b69a6fa036380dd82a0f067f8e97178a8da04f68a9c4a9eb4c10f5c432c7ad`  
		Last Modified: Wed, 13 Dec 2023 02:39:17 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148841d4329f6dd8e152b2fc00676a9c4becd06e9c761400458c7b2d46438314`  
		Last Modified: Wed, 13 Dec 2023 02:39:17 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f8b0320cdf29c8f5349e14ec28542bd3c57d39b3d69d580de8ec462540d01`  
		Last Modified: Wed, 13 Dec 2023 02:39:17 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b20c979eb5abf12332bf27e4b1aa8d06c7b7d6253b88d67681f13191b2ed1f5`  
		Last Modified: Wed, 13 Dec 2023 02:39:17 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a3dce4dbfd8b7dec08593b9d5c29404f49689161151ee3dda24b973f91dbe`  
		Last Modified: Wed, 13 Dec 2023 02:39:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbc07c2849a4af7257c854c4fbd200cea57e1d10b82012dfcbe9a675b6fdcc0`  
		Last Modified: Wed, 13 Dec 2023 02:39:15 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6842cf61f849c09c274f395d1e08b1196c674d9a59c34ddc4a9eb69e190b9d`  
		Last Modified: Wed, 13 Dec 2023 02:39:15 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6823cd563e14b3750718450028cc7815abe14745863b57adc3e7524f3cdbfcb`  
		Last Modified: Wed, 13 Dec 2023 02:39:15 GMT  
		Size: 290.0 KB (289982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae3d36b08abac2ea5a039a22621cc239126e2c32070f73be4efaacfc3c81c91`  
		Last Modified: Wed, 13 Dec 2023 02:39:15 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
