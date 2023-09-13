## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:4e0879a2422f5309c4ed33c36438e076aa198dc89228e2dc8a56369b86fac7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
