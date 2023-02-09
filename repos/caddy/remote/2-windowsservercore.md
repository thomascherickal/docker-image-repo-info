## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:0824e61dd8be6c1fa86bcf0faf1d4c5d8a41c047e0d4bf9ec8bbb73f243adaf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
