## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9ba0b87da005cab3abb5809cf21dc3b12f8fac8e83c43179846866ba77a9883f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
