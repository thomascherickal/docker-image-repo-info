## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:618d9f501fb56f3d12f4566a58de1afafc1a3920ba686c84cc2e1134d1bf41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
