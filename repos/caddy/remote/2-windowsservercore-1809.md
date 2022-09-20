## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:d72096b4f20f61bf463d816b153a0ba485aa4b8c1cf85248519949102a8f68b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:d7db9b1b3cdab1567bf91ad1f3b49525813d2a01171c5887ad5b9025081d9eb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7683f48122d450dec80a02a03dab974285800188fd6984e74c4f490274213957`
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
# Tue, 20 Sep 2022 21:15:49 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 21:17:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('49582519293819fd4086540aa83428f75af7074882056b6cbe7ab29038f11587f9b6ea2bd68de583e4e99e7afb5bd42ea943e81065a1dc0b5f0b3057f7a0da0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 20 Sep 2022 21:17:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 20 Sep 2022 21:17:13 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 20 Sep 2022 21:17:14 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 21:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 21:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 21:17:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 21:17:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 21:17:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 21:17:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 21:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 21:17:21 GMT
EXPOSE 80
# Tue, 20 Sep 2022 21:17:22 GMT
EXPOSE 443
# Tue, 20 Sep 2022 21:17:23 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 21:17:24 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 21:18:14 GMT
RUN caddy version
# Tue, 20 Sep 2022 21:18:15 GMT
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
	-	`sha256:c321b986d79e251e57d07601b1c55fa13d2b45ef9de8768ddd9c3cadf89b5852`  
		Last Modified: Tue, 20 Sep 2022 21:22:08 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf735c6fd9e641b384edbfe6ba5ceb05307d107b7372cef5dedafaebb69506`  
		Last Modified: Tue, 20 Sep 2022 21:22:11 GMT  
		Size: 14.9 MB (14904011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b3aeef135416d6c6356531b8eaccd78775b16fcaa39e74906684285a19c21`  
		Last Modified: Tue, 20 Sep 2022 21:22:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75af89279a5fa4169d839cc86b46b4637eecdbd7dd41f69bbd7d8c1f5a39cd20`  
		Last Modified: Tue, 20 Sep 2022 21:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dae98dc0855ebe2c41992478fe662d776b39954dcf97e87b78e6202a07d10df`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524294a3cdce5ce2e8ab0086f1e8151f01a958c7a435af7f2721f3de00908b99`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5deb16e98516130995b20182b32b6320eee2a629d6c2336a51fa5c6d28f8fe90`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6926d330fbe8a23a3cff8957075f0cca0e889082baa27fd52c1070f50decbd`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa7a22d1f59d8d1a3d0b6ac4fa4aa729c7478491ee8cc124be7d7ba7097deb`  
		Last Modified: Tue, 20 Sep 2022 21:22:04 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea66fc4101419cb9eba83238cf945eecca732dbd52f2184b6e2b967f92d49f3f`  
		Last Modified: Tue, 20 Sep 2022 21:22:04 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df966808bb1c7e3b916a530158feefcfce8699034d9c07c7b9ad3c5f50aac6b3`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257d1dd36c1f128bb7805c57ef3c339189749d51e663771e4a8d3b7d8437390`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7c526b2d38f043453b8220aefaeee679e3ff7ae00b2e55fbd5218a12e4333`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c8e0ffe60e71db7689f6f05bb71bc3d81192a83166bddf2b57445b6459a5e`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab8b8dbcb7997076b6b7f02563628c13f0ad49a0dedd0788c0cb25d9df49564`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bc4d651137a0c053a4c2a929ce35948c90e2ec719b7a434a4e23cd45ff2db7`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba74362d5c5ebd167aaaeafb147886f6089088c081a52fa88939414a38e49778`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 307.7 KB (307722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b417cb891c81d0327c5a5fec64ea647390aca9869e325a1bf78f08c1b21e3d9e`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
