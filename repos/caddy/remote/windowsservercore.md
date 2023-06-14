## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:46f7c5c6bcf219fae3376813b3f15821555f3fcaf5eb55973c762710a2418c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4499; amd64
	-	windows version 10.0.20348.1787; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull caddy@sha256:c621df0c0c615f05c76f38de2bfaabf0a91ef6fdab2739ee6e75b1c80bc3e603
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1665839112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975a0e757723bc421f0d1dd119f42c8b1f4388dd59ba125d504d6ea6291ab373`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:39:16 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jun 2023 20:39:17 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 14 Jun 2023 20:40:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jun 2023 20:40:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jun 2023 20:40:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jun 2023 20:40:02 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 14 Jun 2023 20:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jun 2023 20:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jun 2023 20:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jun 2023 20:40:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jun 2023 20:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jun 2023 20:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jun 2023 20:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jun 2023 20:40:09 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:40:09 GMT
EXPOSE 443
# Wed, 14 Jun 2023 20:40:10 GMT
EXPOSE 443/udp
# Wed, 14 Jun 2023 20:40:11 GMT
EXPOSE 2019
# Wed, 14 Jun 2023 20:40:28 GMT
RUN caddy version
# Wed, 14 Jun 2023 20:40:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91aebdd77c82ecb5ff75a9cddf1b0c5c494276cd36ac69bf04802bb84b00f32e`  
		Last Modified: Wed, 14 Jun 2023 20:48:13 GMT  
		Size: 318.2 KB (318154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f958341ead38541da55d41be736221d7186b9c5a03ef33eae2cd92ce820b88`  
		Last Modified: Wed, 14 Jun 2023 20:48:13 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168ae31cf39b5ccf32926fbaa5a018eed778a5be5f768fdce2899471bee74446`  
		Last Modified: Wed, 14 Jun 2023 20:48:16 GMT  
		Size: 14.6 MB (14606514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e95f7343cea45e725e6a48b265068c44e92eb2778548929089303bc4333ac`  
		Last Modified: Wed, 14 Jun 2023 20:48:13 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916fbee90d720f77bba554088029b91bc3b44c8549c661ac1e955475d1438b14`  
		Last Modified: Wed, 14 Jun 2023 20:48:11 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b9920c996993f252b238ffe47b17075ef26014e0dfa22723cc0d38d7cf6d4`  
		Last Modified: Wed, 14 Jun 2023 20:48:11 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f727c9a57c33d314f00cdef9d1b22f30a63308a4e562dadefa81d8dad021949f`  
		Last Modified: Wed, 14 Jun 2023 20:48:11 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fbd7499221cd2a87d6d385a8e412050f6d5c7606443e952910b57d4f4e1989`  
		Last Modified: Wed, 14 Jun 2023 20:48:11 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35194cf00a5e7d2c28afb7fdc64de6db74e59581a5f30f514b9f29edd28939de`  
		Last Modified: Wed, 14 Jun 2023 20:48:11 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16e46a6f615676d3946e097299a1c82f86211a2463776e10f68a2a05fc6a311`  
		Last Modified: Wed, 14 Jun 2023 20:48:10 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf5724f09e7966a7e7886c469dc8c2470ea7bbcfa9b4eeec95b73fef8f26c42`  
		Last Modified: Wed, 14 Jun 2023 20:48:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bd6bc490f7da0b739b2b25f71090a3324cb9648e869b4f5a27b1b63517668b`  
		Last Modified: Wed, 14 Jun 2023 20:48:09 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbc588bb9987308f0adb33c6e36f4d9766fde013f98d17e2f909caff6cb5897`  
		Last Modified: Wed, 14 Jun 2023 20:48:09 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40763a012b4c3f58238650195be84e50cafd7de053d999a32c2175657a21e970`  
		Last Modified: Wed, 14 Jun 2023 20:48:09 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6091f6b2745fd2b49574f08af49b345ec2108578d1b1ce8006e4524529caa18`  
		Last Modified: Wed, 14 Jun 2023 20:48:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419930b01b938f721a285b03999ba039f99607dcc3ba19529fb1d5bf5c0166e6`  
		Last Modified: Wed, 14 Jun 2023 20:48:07 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fc064b7b862137e129898a180e7e74137393a87dc1acaed75069c642bfda5c`  
		Last Modified: Wed, 14 Jun 2023 20:48:07 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33234895173b731192fd8f861f39f25b062c945571232b507edd5e6ccd07df`  
		Last Modified: Wed, 14 Jun 2023 20:48:07 GMT  
		Size: 271.8 KB (271821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8059ad67fb965928b14f9a12e4368e84748fdce324dc6a91df883b6c24807923`  
		Last Modified: Wed, 14 Jun 2023 20:48:07 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull caddy@sha256:5cb69b4f77afd85d00bf9c68d5d2638ea0c6b12e120605cd3705fd30aa9882dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1403829483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5889043836cab03be869ed6778798bcd412013790fa98ce03252148560bea1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:41:08 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jun 2023 20:41:08 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 14 Jun 2023 20:41:35 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jun 2023 20:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jun 2023 20:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jun 2023 20:41:38 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 14 Jun 2023 20:41:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jun 2023 20:41:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jun 2023 20:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jun 2023 20:41:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jun 2023 20:41:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jun 2023 20:41:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jun 2023 20:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jun 2023 20:41:44 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:41:45 GMT
EXPOSE 443
# Wed, 14 Jun 2023 20:41:46 GMT
EXPOSE 443/udp
# Wed, 14 Jun 2023 20:41:47 GMT
EXPOSE 2019
# Wed, 14 Jun 2023 20:42:05 GMT
RUN caddy version
# Wed, 14 Jun 2023 20:42:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2437621545ffec6b315ad0cb9799fd85bf9655afe894d2d6fc320c0b6fbe6774`  
		Last Modified: Wed, 14 Jun 2023 20:48:38 GMT  
		Size: 326.8 KB (326823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24752713ae53dff67cb6b2b506f30884d0b2f4f3e401769603aeee5f1f48076e`  
		Last Modified: Wed, 14 Jun 2023 20:48:38 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4f0d2be9ceb8a1bf489217e5f924cd21a74e5345077c1aead1c300ca28a3e5`  
		Last Modified: Wed, 14 Jun 2023 20:48:41 GMT  
		Size: 14.6 MB (14601907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4570118706989654c9a2490776869bc687a6a0438f1371fec752e17a95bcec`  
		Last Modified: Wed, 14 Jun 2023 20:48:38 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d25d34aed9f6896b71705301526038d6f2d34288b59bdd7922248dd8cf102a`  
		Last Modified: Wed, 14 Jun 2023 20:48:36 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dda55e575fd42cbffb7b6ece85683f49246e238eb94df222fffbc3f56414c35`  
		Last Modified: Wed, 14 Jun 2023 20:48:36 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9626f7a6278d3e03edb37377977f8417a4c771d18a083e556acd2a5310d3574b`  
		Last Modified: Wed, 14 Jun 2023 20:48:36 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11dfc4f97e26258eea4a7f0b5d9859d0331056f93c5b45e12423ccb488f1347`  
		Last Modified: Wed, 14 Jun 2023 20:48:36 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6566184fca648d3955d2cfaa37f5d2ce122533682f383c02413c560e5ca4a68`  
		Last Modified: Wed, 14 Jun 2023 20:48:36 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e463fe90d2b606446d26bd0a2bbd0e37f1905b5a8def4e3ffa48cf5b09be99`  
		Last Modified: Wed, 14 Jun 2023 20:48:34 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaca5c69962bf77ba81febf6bf8076265c2a6c6c40bf34a2d90cd86eed06b90`  
		Last Modified: Wed, 14 Jun 2023 20:48:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d352b1f01eed948427de035e4251cb0e9d5bf96725e725c53b3f1fb394d83`  
		Last Modified: Wed, 14 Jun 2023 20:48:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9017a99cd9882dc14e92314b80cc1ddab7485e7397a2e3a490bcf475cb8cae67`  
		Last Modified: Wed, 14 Jun 2023 20:48:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cbe6b8483914ed7ffbb2237f7b4497df93e2b8248244fa74d7d049893807d3`  
		Last Modified: Wed, 14 Jun 2023 20:48:34 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0be49dd9a5d93c9ef20a09ca37e5ae516d753692006f0a64ddd6ef10d65ad61`  
		Last Modified: Wed, 14 Jun 2023 20:48:32 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4482041b3d8af6ae73707f69ac9fb2ebfc345d4b0b8b20317687cee91323a3`  
		Last Modified: Wed, 14 Jun 2023 20:48:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f9b306a26fe3083f1120d6ff251abed4a8d709475952bb65bd5529a55dfce5`  
		Last Modified: Wed, 14 Jun 2023 20:48:32 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec57d08cb236334bbc10b100b17a5d7f07b1016701a01985a655fb132be4d35`  
		Last Modified: Wed, 14 Jun 2023 20:48:32 GMT  
		Size: 279.8 KB (279781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483af7acbb45a925c9da3fe4c94e52047afb0f33ce30b665ceeffe848611d072`  
		Last Modified: Wed, 14 Jun 2023 20:48:32 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
