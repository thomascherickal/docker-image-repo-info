## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f65a2a6e954346897215a9d2fa42d57afe06720d80aa6f5ee846aea9dd2343e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
