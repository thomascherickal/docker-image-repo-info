## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:7c8910562b78f49c3a2f608132f963d70e34352d7b1eba277e11d71c4aadd90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull caddy@sha256:23906c96e8647871d54638ee95201b15a6780bd5c5a55e1910f1cce47f51327a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2075748892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd668c1e74ca31419de6a4894168996b6be13d2cfb6dda297f76f1f0e82af65`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 02:30:40 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Dec 2023 02:30:41 GMT
ENV CADDY_VERSION=v2.7.6
# Wed, 13 Dec 2023 02:32:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.6/caddy_2.7.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b2321473be1da500a8f6e4276aed03b11946e3758b792a3e9ba50c07246456d64d7da931d6d58be43e6d3cfd07c1ad68f6838df8e090bd5d212224a9bf94daec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Dec 2023 02:32:02 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Dec 2023 02:32:03 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Dec 2023 02:32:04 GMT
LABEL org.opencontainers.image.version=v2.7.6
# Wed, 13 Dec 2023 02:32:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Dec 2023 02:32:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Dec 2023 02:32:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Dec 2023 02:32:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Dec 2023 02:32:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Dec 2023 02:32:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Dec 2023 02:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Dec 2023 02:32:11 GMT
EXPOSE 80
# Wed, 13 Dec 2023 02:32:12 GMT
EXPOSE 443
# Wed, 13 Dec 2023 02:32:13 GMT
EXPOSE 443/udp
# Wed, 13 Dec 2023 02:32:13 GMT
EXPOSE 2019
# Wed, 13 Dec 2023 02:33:19 GMT
RUN caddy version
# Wed, 13 Dec 2023 02:33:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc953d49171296238d791f543a2a026383540af60c9b10cc72446745ea9e517`  
		Last Modified: Wed, 13 Dec 2023 02:38:55 GMT  
		Size: 466.4 KB (466376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5091a1fcf41a799b6b5325321d36e20072d566027eeecc072788a9a3c3afbf0b`  
		Last Modified: Wed, 13 Dec 2023 02:38:54 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d0c21ea3d396314641058b6087c719f00acf6e81a122d0308c76705b454c5a`  
		Last Modified: Wed, 13 Dec 2023 02:38:58 GMT  
		Size: 15.3 MB (15282292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c1ffefa6eaf8ceb9b6964a75043f3440c260e5ef8a7757a4902bbd87b5a11`  
		Last Modified: Wed, 13 Dec 2023 02:38:54 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209a9db6a8a0e20f16c07fa90f84ff5f0fbcf8896b719c5282405503804e4975`  
		Last Modified: Wed, 13 Dec 2023 02:38:53 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3e6508c4f7300255ca275dc9fa4b8ff9f4e4ff4e6c552afee4d03305e571f8`  
		Last Modified: Wed, 13 Dec 2023 02:38:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a096f7d34249fda9c90244912f35e632dc8c3c50a830c1d3dc6d5d2234264`  
		Last Modified: Wed, 13 Dec 2023 02:38:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee679db41077812368c0ee8780348a81cc00878e2848106d2b022cfa25222615`  
		Last Modified: Wed, 13 Dec 2023 02:38:52 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61da3eb55b53d10c6d39556e06adcd87b1e813dbf6e7c0c09a4a1fcd3c1a02af`  
		Last Modified: Wed, 13 Dec 2023 02:38:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67d27f68c7ff3cf8ec13fd0ae72ac89b781c819f1959e16c22101faa49884a1`  
		Last Modified: Wed, 13 Dec 2023 02:38:51 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b0c532fc98f8438a57e314863455c2812c5f8273718a387893d58b1eae45a7`  
		Last Modified: Wed, 13 Dec 2023 02:38:51 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb76494edec3148a22e8826aa2cceb75046d74559b7fe31713da82a5504d187`  
		Last Modified: Wed, 13 Dec 2023 02:38:50 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621db1494746176522163d644f8f6d572003928346b37dfea1118539767375bf`  
		Last Modified: Wed, 13 Dec 2023 02:38:50 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e621e03d954adf248bd9ddcdfe28108be9204a2f010bc44cd49534bc26d10c`  
		Last Modified: Wed, 13 Dec 2023 02:38:50 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb96c188ceb57176f56af8649f49ebde260394730cc2ee6bd5a10634d6676bc`  
		Last Modified: Wed, 13 Dec 2023 02:38:48 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e2237c5f2e48a944f2cdc493acec61ca707749a0d33362f62a1162e6967f7f`  
		Last Modified: Wed, 13 Dec 2023 02:38:48 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b904a8ec5a95b1df9b634285424830763de3a36377f8f97be9383346cd82022`  
		Last Modified: Wed, 13 Dec 2023 02:38:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720ae7bbabfc6a290ea47a42a976c34545f19465895a8dee1bd94b9f6351d9ae`  
		Last Modified: Wed, 13 Dec 2023 02:38:49 GMT  
		Size: 269.0 KB (268985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4235be6cdbcf40a5350abf8550ae54349cd6889349bacb2c4c6fcdabb02fcb`  
		Last Modified: Wed, 13 Dec 2023 02:38:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
