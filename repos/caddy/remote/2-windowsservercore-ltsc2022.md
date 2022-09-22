## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:391c3e9d6a79f66b9cfdc3800ac89da113665ef28bd627bc2ae077a8fdffa0d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
