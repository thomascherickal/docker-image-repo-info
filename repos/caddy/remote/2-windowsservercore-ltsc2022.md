## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8b07fddd6e884d7cd57b16fe8dfc8d764e50c606b804ace49eac539534eba9da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
