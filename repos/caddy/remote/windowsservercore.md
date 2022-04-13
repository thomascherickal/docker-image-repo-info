## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
