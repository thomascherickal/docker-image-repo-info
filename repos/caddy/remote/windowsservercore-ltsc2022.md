## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:88a75e54141f2e7531d3262b5a00a17002af383f24e29dab09212e4cbbfa2fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:a3894222673d46b3e350553c6b7d4f92ab27b85a87fa1f773e9b090d5774ca9e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2252723203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063f1879bd2783934ad3ac23aa37bf45f19be756f6b018f4c3a67d2d4a759c7c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:31:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 10 May 2022 23:31:42 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:32:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('4294796c4bd4bed0c593d83606a5413de30f35f88d624e1b1e5b6cd8672ffbcc7a689d7ce4ef30c1abea0e95eda62220faac15d2a6aca0c3e2b418abe7a74118')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 10 May 2022 23:32:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 10 May 2022 23:32:12 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 10 May 2022 23:32:13 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Tue, 10 May 2022 23:32:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 10 May 2022 23:32:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 10 May 2022 23:32:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 10 May 2022 23:32:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 10 May 2022 23:32:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 10 May 2022 23:32:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 10 May 2022 23:32:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 10 May 2022 23:32:21 GMT
EXPOSE 80
# Tue, 10 May 2022 23:32:22 GMT
EXPOSE 443
# Tue, 10 May 2022 23:32:23 GMT
EXPOSE 2019
# Tue, 10 May 2022 23:32:42 GMT
RUN caddy version
# Tue, 10 May 2022 23:32:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9baa8a196af04dc55746ee82c0774537bce72a589b75d9efce1a4680f03e35`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 616.1 KB (616130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe60c7e90fdaeffa9bce60d9a7c7b340dedc357bfb70a2ce8c6d7b8bd0e74a11`  
		Last Modified: Tue, 10 May 2022 23:36:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955bea173999b55d2087a27b9cc80e92bf168918c6e892175c2a75bdbfac933`  
		Last Modified: Tue, 10 May 2022 23:36:07 GMT  
		Size: 14.2 MB (14224642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1ab4508d5347b929d5a33f71e0f24f653e61c147260200d32e3bd7cdd2340`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8044ca4427c5edfee653001205397a2cc33f8fb4416c16c4a4936317c572ed`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f144416d38a1aa75558e0b93b88fcb3de122ee88349826ee99d596e1b00d9cc0`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edbcceba80e7a70e44725926012bb70624bb0ae91c85db2766ca2e4c5a5d7c`  
		Last Modified: Tue, 10 May 2022 23:36:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd90105a2a3136e4d25d0add2b6fbe5798d51588215367128f1566d66b255289`  
		Last Modified: Tue, 10 May 2022 23:36:01 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e448ed08c6c6ca9f854cb7014ea2e79c04e83f1905f78f578b67303b709fa3`  
		Last Modified: Tue, 10 May 2022 23:36:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d49b1b3778cd2ebf32521f530e29275a9a473afa997654b32338ff4349bf5c`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2112945425b7d069bc5705be1345e5ad6e27206e1531b10d0bc92d9c69ea9c3`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7243327255edd82b277f456085138a672f5a43d616e80f73156c8eb31139121d`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a14330360d7ab3af40d4fb6f2de975e42e05f8e4cb064cc49fe1d9446e6b1`  
		Last Modified: Tue, 10 May 2022 23:35:59 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808ce6a15ca3e6ad031229bcad8a3ed69171a7005c05ef4e77ffcfd777e9d1f7`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfcf611e614d42a256d103775233f59ab7bb6ad0b00ca2f915bf739600f8d6`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3811622d464d497ce363eed806c75f9b994cd1d04b3009b2d0671af2863ebd0`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b006092864e6cfdfedd054a2635236c62958e97de81c720d9e38772276ee11`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 325.9 KB (325870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afb0ece27a359f16126f263176baa74c3d3f2f2733cce186e4e31ad0eca4f8`  
		Last Modified: Tue, 10 May 2022 23:35:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
